# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/)

## [Unreleased]
### Added
 - Creation of the initial Changelog file
### Changed
 - Modification of build stage and steps
 - Update to Readme format and additonal context
 - Update plugin versions for Maven
 - Change of repository name and location to public oss.jfrog.org
 - Change of bintray usage to allow for snapshot deployments
 - Additional configuration and execution for the allowance of Tar file uploads of dockerimages
 - Additional settings to publish to mavenl central for released binaries
 
### Removed
 - Removal of bintray usage for internally generated artifacts as all binaries will be created in OpenSource
 - Removed Unrequired Docker configuration in pom file

## [0.2.4] - 2017-05-05
### Added
 - Copyright information to cpsd created scripts.
 - Additional distribution management location for internally generated binaries to be published to public domain

### Removed
 - Removed OSS sonatype staging maven location from Repository Management section
 - Removed upload of docker tar file execution strategy
 

## 0.2.3 - 2017-05-05
### Added
 - Initial addition of the distribution management and properties

[Unreleased]: https://github.com/dellemc-symphony/root-parent/compare/0.2.4...HEAD
[0.2.4]: https://github.com/dellemc-symphony/root-parent/compare/0.2.3...0.2.4

