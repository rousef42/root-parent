# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/)

## [Unreleased]

## [1.0.1] - 2017-07-25
### Added
 - Properties [palantir/releases](http://palantir.bintray.com/releases) for added public repository

## [1.0.0] - 2017-06-23
### Added
 - Creation of the initial changelog file.
### Changed
 - Modification to build stage and procedure.
 - Readme format and additional context.
 - Plugin versions for Maven.
 - Snapshot repository name and location to public [oss.jfrog.org/oss-snapshot-local](https://oss.jfrog.org/list/oss-snapshot-local).
 - Release repository name to public [dell-emcs-cpsd/maven-central-prepare](https://dl.bintray.com/dell-emc-cpsd/maven-central-prepare).
 - Bintray usage to allow for snapshot deployments.
 - Additional configuration and execution for the allowance of TAR file uploads of Docker images.
 - Additional settings to publish to Maven Central for released binaries.
 
### Removed
 - Bintray usage for internally generated artifacts as all binaries will be created in opensource.
 - Unrequired Docker configuration in the POM file.

## [0.2.4] - 2017-05-05
### Added
 - Copyright information to CPSD created scripts.
 - Additional distribution management location for internally generated binaries to be published to public domain.

### Removed
 - OSS sonatype staging Maven location from repository management.
 - Upload of Docker TAR file execution strategy.
 
## 0.2.3 - 2017-05-05
### Added
 - Distribution management and properties.

[Unreleased]: https://github.com/dellemc-symphony/root-parent/compare/1.0.1...HEAD
[1.0.1]: https://github.com/dellemc-symphony/root-parent/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/dellemc-symphony/root-parent/compare/0.2.4...1.0.0
[0.2.4]: https://github.com/dellemc-symphony/root-parent/compare/0.2.3...0.2.4

