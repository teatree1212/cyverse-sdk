# Change Log
All notable changes to this project will be documented in this file.

## Version 1.2.2 - 01/02/2017
### Added
* Nothing

### Changed
* Synced to latest Agave CLI

### Removed
* Nothing

## Version 1.2.1 - 12/16/2016
### Added
* Nothing

### Changed
* Synced to latest Agave CLI

### Removed
* Nothing

## Version 1.2.0 - 10/05/2016
### Added
* Support for Lonestar5 at TACC

### Changed
* Private TACC systems now use gateway hosts in order to support Multifactor Authentication
* System enrollment now relies on a dedicated Python 2.6.x script rather than sed
* Revised onboarding tutorial to support SSHKEYS for TACC systems in favor of passwords, which are deprecated

### Removed
* Temporarily deprecated support for TACC Maverick
* Removed private system support for Lonestar4

## Version 1.1.4 - 09/29/2016
### Added
* Nothing

### Changed
* Updated to track latest agaveapi/cli ece6d2043dd734aedfed10fe10cb900f7e5c9fb9

### Removed
* Nothing

## Version 1.1.2 - 06/15/2016
### Added
* Nothing

### Changed
* Updated to latest Agave CLI featuring `jobs-kick` command + fixes

### Removed
* Nothing

## Version 1.1.1 - 05/10/2016
### Added
* cyverse-sdk-info learned to check the SDK version and update if necessary

### Changed
* Official Ubuntu-based cyverse/cyverse-cli image is automagically available at Docker Hub with every release

### Removed
* Nothing

## Version 1.1.0 - 05/06/2016
### Added
* Nothing

### Changed
* Moved to use agaveapi/cli as basis for the SDK

### Removed
* Nothing

## Version 1.0.10 - 04/06/2016
### Added
* Nothing

### Changed
* Incorporated @wjallen updates and improvements to Agave foundation-cli

### Removed
* Nothing

## Version 1.0.9 - 03/09/2016
### Added
* Nothing

### Changed
* Fixed an issue with tacc-systems-create where the final listing of systems would fail. This was due to the script calling to Agave's hosted json-mirror over http. Problem was addressed by changing url to https.

### Removed
* Nothing

## Version 1.0.8 - 02/15/2016
### Added
* iplantc/cyverse-cli:1.0.8 released to Dockerhub

### Changed
* Substantial updates to docs reflecting state of Agave API at Cyverse
* Fixed Docker image cache directory amnesia
* Fixed broken cyverse-sdk-info

### Removed
* Nothing

## Version 1.0.7 - 02/15/2016
### Added
* Nothing

### Changed
* Fixed virtual rootDir for storage and compute systems at TACC
* Pinned executionSystem logins to specific login node on each system

### Removed
* Nothing

## Version 1.0.6 - 02/14/2016
### Added
* Nothing

### Changed
* Removed support for cyverse-sdk-info in Makefile

### Removed
* cyverse-sdk-info (for now)

## Version 1.0.5 - 02/13/2016
### Added
* Nothing

### Changed
* Added check for empty values in tacc-systems-create
* Added check for BSD vs Linux sed in Makefile
* Renamed cyverse-cli-info to cyverse-sdk-info
* Fixed an issue where TMPDIR was not defined in tacc-systems-create

### Removed
* Nothing

## Version 1.0.4 - 02/07/2016
### Added
* docker-clean make target in Makefile

### Changed
* cyverse-cli image now contains python 2.7.11 (or higher) to support JSON parsing
* updated BUILD to reflect docker-specific make targets

### Removed
* Nothing

## Version 1.0.3 - 02/07/2016
### Added
* Completed Docker support with addition of docker and docker-release make targets
* jsonpki command for serializing private and public keys

### Changed
* Nothing

### Removed
* Nothing

## Version 1.0.2 - 02/05/2016
### Added
* cyverse-cli-info command to report API, tenant, etc
* Support for TACC global WORK storageSystem
* Support for Lonestar5 executionSystem


### Changed
* Fork of iplant-agave-sdk, placed under active version management
* Fixed installation instructions

### Removed
* Support for Lonestar4 executionSystem
* Support for Wrangler executionSystem (will return soon)
