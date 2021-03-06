# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]
### Added

### Changed

### Fixed

## [2.1.2] - 2016-04-25
### Added
* Redesigned Packaging feature, including new system/package API and artisan commands for import and export.
- Added Redis and Memcached config options to dreamfactory:setup command 
- Added Memcached config values in environment 
- Updated dreamfactory:import-pkg command to use new package format
- Updating initial setup to import any packages available
- Added artisan dreamfactory:config-hhvm command to create hhvm config file 
- Basic support for www-form-urlencoded payload in API requests
- Add rewrite rule to allow basic auth on AWS cloud and VM. 

### Changed
- Cleanup service providers 
- Handling file stream output using StreamedResponse 

### Fixed

## [2.1.1] - 2016-03-14
### Added
- More env config option in setup command
- Now allowing login with JWT passed as URL parameter
- Added log level support, see DF_LOG_LEVEL in .env-dist for options

### Changed
- Upgraded Laravel framework to 5.2
- File Manager app is now standalone composer pulled app

### Fixed

## [2.1.0] - 2016-01-29

### Changed
- **MAJOR** Updated code base to use OpenAPI (fka Swagger) Specification 2.0 from 1.2
- Replacing old swagger UI with fork of latest Swagger 2.0 UI

## [2.0.4] - 2016-01-06
### Fixed
- Bug fixes for df-core dependencies
- FileManager app to include OpenStack Object Storage

## [2.0.3] - 2015-12-22
### Added
- Laravel Homestead setup for quick launch of testing environment.
- More environment changes for managed instances, including limit tracking.

### Changed
- Using 'AES-256-CBC' as default Cipher in config/app.php, mirroring Laravel 5.1. 
For older installs, see DF_CIPHER in .env or .env-dist for more details.

### Fixed
- SQLite storage location for managed instances.

## [2.0.2] - 2015-11-30
### Added
- New migration check for upgrade scenarios.
- AD enhancements.
- This changelog!

### Changed
- Rework AccessCheck middleware, move AuthCheck to global for easier usage in enterprise scenarios.
- Email templates back to original html/text based instead of blade.
- Composer additions.

## [2.0.1] - 2015-10-28
### Fixed
- A bug that prevented proper logout when token is invalid.

## 2.0.0 - 2015-10-27
First official release of the new open-source DreamFactory project.

[Unreleased]: https://github.com/dreamfactorysoftware/dreamfactory/compare/2.1.0...HEAD
[2.1.0]: https://github.com/dreamfactorysoftware/dreamfactory/compare/2.0.4...2.1.0
[2.0.4]: https://github.com/dreamfactorysoftware/dreamfactory/compare/2.0.3...2.0.4
[2.0.3]: https://github.com/dreamfactorysoftware/dreamfactory/compare/2.0.2...2.0.3
[2.0.2]: https://github.com/dreamfactorysoftware/dreamfactory/compare/2.0.1...2.0.2
[2.0.1]: https://github.com/dreamfactorysoftware/dreamfactory/compare/2.0.0...2.0.1
