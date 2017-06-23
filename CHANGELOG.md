# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/)

## [Unreleased]
### Added
 - Creation of the initial Changelog file
### Changed
 - Modification to build stage and procedure
 - Update to readme format and additional context
 - Update the plugin versions for Maven
 - Change of snapshot repository name and location to public [oss.jfrog.org/oss-snapshot-local](https://oss.jfrog.org/list/oss-snapshot-local)
 - Change of release repository name to public [dell-emcs-cpsd/maven-central-prepare](https://dl.bintray.com/dell-emc-cpsd/maven-central-prepare)
 - Change of bintray usage to allow for snapshot deployments
 - Additional configuration and execution for the allowance of TAR file uploads of Docker images
 - Additional settings to publish to Maven Central for released binaries
 
### Removed
 - Removal of bintray usage for internally generated artifacts as all binaries will be created in opensource
 - Removal of unrequired Docker configuration in the POM file

## [0.2.4] - 2017-05-05
### Added
 - Copyright information to CPSD created scripts
 - Additional distribution management location for internally generated binaries to be published to public domain

### Removed
 - Removed OSS sonatype staging Maven location from repository management
 - Removed upload of Docker TAR file execution strategy
 
## 0.2.3 - 2017-05-05
### Added
 - Initial addition of the distribution management and properties

[Unreleased]: https://github.com/dellemc-symphony/root-parent/compare/0.2.4...HEAD
[0.2.4]: https://github.com/dellemc-symphony/root-parent/compare/0.2.3...0.2.4

