# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- SHA512 Whirlpool hashing algorithm
- phpass hashing implementation
- Support for salt column

### Fixed
- Table and column autocomplete in settings panel

## [v4.0.0-rc2]
### Added
- User active column

### Changed
- Fixed "Use of undefined constant" error for Argon2 Crypt with PHP below 7.2.

## [4.0.0-rc1]
### Added
- New hashing algorithms: Argon2 Crypt (PHP 7.2 and above), Blowfish Crypt, Courier base64-encoded MD5, Courier base64-encoded SHA1,
  Courier base64-encoded SHA256, Courier hexadecimal MD5, Extended DES Crypt, SHA256 Crypt,
  SHA512 Crypt, SSHA512, Standard DES Crypt
- Option to allow users to change their display names
- Option to allow user to change its avatar 
- Database query results cache
- Option for group display name
- Option for group is admin flag

### Changed
- The whole core implementation, which is NOT COMPATIBLE with the previous versions.
- Minimum supported PHP version - 7.0

## Removed
- MySQL ENCRYPT() hashing implementation - Function is deprecated as of MySQL 5.7.6 and will be removed in a future MySQL release.
- MySQL PASSWORD() hashing implementation - Function is deprecated as of MySQL 5.7.6 and will be removed in a future MySQL release.
- Redmine hashing implementation - Cannot implement in new core system.
- User active column - Use database view instead
- Domain support

## [3.1.0] - 2018-02-06
### Added
- Column autocomplete for PostgreSQL
- Currently supported parameters in README.md
- SALT support for password algorithms "system" and "password_hash"

### Changed
- Updated README.me file
- Nextcloud 12 & 13 support
- Moved files to be more on the standard places
- Renamed some files to be more standard like
- Source code changes to be more standard like (max 80 characters)

### Fixed
- Column autocomplete in "Groups Settings"
- Security fix for password length sniffing attacks
- Small bug fixes

## Removed
- Code for supervisor mode

## 2.4.0 - 2017-12-26
### Added
- This CHANGELOG.md file
- Support for PHP 7
- SHA1 hash algorithm support
- Groups option
- Supervisor option

### Changed
- Supported version of ownCloud, Nextcloud: ownCloud 10, Nextcloud 12

[Unreleased]: https://github.com/nextcloud/user_sql/compare/v4.0.0-rc2...develop
[v4.0.0-rc2]: https://github.com/nextcloud/user_sql/compare/v4.0.0-rc1...v4.0.0-rc2
[4.0.0-rc1]: https://github.com/nextcloud/user_sql/compare/v3.1.0...v4.0.0-rc1
[3.1.0]: https://github.com/nextcloud/user_sql/compare/v2.4.0...v3.1.0
