pipeline {
    parameters {
       choice(choices: 'ON\nOFF', description: 'Please select appropriate flag', name: 'Deploy_Stage')
    }	
    agent {
        node {
            label 'maven-builder'
            customWorkspace "workspace/${env.JOB_NAME}"
        }
    }
    environment {
        GITHUB_TOKEN = credentials('git-02')
    }
    options {
        skipDefaultCheckout()
        buildDiscarder(logRotator(artifactDaysToKeepStr: '30', artifactNumToKeepStr: '5', daysToKeepStr: '30', numToKeepStr: '5'))
        timestamps()
        disableConcurrentBuilds()
    }
    tools {
        maven 'linux-maven-3.3.9'
        jdk 'linux-jdk1.8.0_102'
    }
    stages {
        stage('Checkout') {
            steps {
                doCheckout()
	        }
	    }
	stage('TravisCI Linter') {
            steps {
                doTravisLint()
            }
        }    
        stage('Compile') {
            steps {
                sh "mvn clean install -Dmaven.repo.local=.repo -DskipTests=true -DskipITs=true"
            }
        }
        stage('Junit Testing') {
            steps {
                sh "mvn verify -Dmaven.repo.local=.repo"
            }
        }
	stage('PasswordScan') {
            steps {
                doPwScan()
            }
        }
       stage('Deploy') {
             steps {
               doMvnDeploy()
             }
        }
        stage('NexB Scan') {
            steps {
                sh 'rm -rf .repo'
                doNexbScanning()
            }
        }
        stage('Third Party Audit') {
            steps {
                doThirdPartyAudit()
            }
        }
        stage('Github Release') {
            steps {
                githubRelease()
            }
        }
    }
    post {
        always {
            cleanWorkspace()   
        }
        success {
            successEmail()
        }
        failure {
            failureEmail()
        }
    }
}
