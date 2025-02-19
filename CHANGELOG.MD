# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.0]

### Added
- Added support for TeamCity Role Assignments for User Groups [#86]
- build-type: support updating the `name` field [#82]
- project: support for updating the name [#81]
- New Build Feature: Golang [#80]
- project-feature/versioned-settings: support for configuring credentialsStorageType [#76]


### Fixes
- Fix panic if parameters is nil [#83]
  
## [1.1.0]  

- Project Features incl update/delete [#73]

## [1.0.0]  

This release is the first major release and includes an upgrade to TeamCity 2019.2.2 as the supported version.
Whenever a major version is bumped, backwards compatibility with previous TeamCity versions aren't guaranteed.

### Changes:
- Updating to use TeamCity 2019.2.2 [#72]
- Added support for TeamCity User Group API [#68]
- Support token auth [#67]

## [0.5.1]

### Added

- Add support for `octopus.push.package` step. It allows creating and pushing packages from [TeamCity to Octopus](https://octopus.com/docs/api-and-integration/teamcity). [#53]

### Fixed
- Issue with serialization and newlines for VCSRoot branchSpec property

### Changed

- (**BREAKING CHANGE**) Move package code from `pkg/teamcity` to `teamcity`.
  - The former structure caused some issues with tooling such as `gocode` and `godef`.
  Since this project follows [go-github](https://github.com/google/go-github) design and conventions, I've adapted the project structure as well.

## [0.4.0] - 2018-10-11

### Added

- Add `GetName()` to Step interface.

## [0.2.0] - 2018-07-16

## [0.1.0] - 2018-07-16

First release.

[//]: # (Release links)
[1.1.0]: https://github.com/leonj1/teamcity-sdk/releases/tag/v1.1.0
[1.0.0]: https://github.com/leonj1/teamcity-sdk/releases/tag/v1.0.0
[0.5.1]: https://github.com/leonj1/teamcity-sdk/releases/tag/v0.5.1
[0.4.0]: https://github.com/leonj1/teamcity-sdk/releases/tag/v0.4.0
[0.2.0]: https://github.com/leonj1/teamcity-sdk/releases/tag/v0.2.0
[0.1.0]: https://github.com/leonj1/teamcity-sdk/releases/tag/v0.1.0

[//]: # (Issue/PR links)
[#53]: https://github.com/leonj1/teamcity-sdk/pull/53
[#67]: https://github.com/leonj1/teamcity/pull/67
[#68]: https://github.com/leonj1/teamcity/pull/68
[#72]: https://github.com/leonj1/teamcity/pull/72
[#73]: https://github.com/leonj1/teamcity/pull/73
[#86]: https://github.com/leonj1/teamcity/pull/86
[#83]: https://github.com/leonj1/teamcity/pull/83
[#82]: https://github.com/leonj1/teamcity/pull/82
[#81]: https://github.com/leonj1/teamcity/pull/81
[#80]: https://github.com/leonj1/teamcity/pull/80
[#76]: https://github.com/leonj1/teamcity/pull/76


