# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- markdownlint-configure-file { "MD024": { "allow_different_nesting": true } } -->

## [2.0.0] 2022-07-15

### Added

- Add [Dependabot](https://github.com/dependabot) in CI.
- This CHANGELOG file.

### Changed

- Upgrade to [Træfik](https://traefik.io/) [v2](https://doc.traefik.io/traefik/migration/v1-to-v2/) syntax.
- Replace CI markdown check.
- Use Docker Compose plugin.
- Put the runner in its own network.

## [1.1.0] 2022-06-22

### Added

- Add Mattermost configuration.

## [1.0.0] 2021-02-09

### Added

- Add a CI to check markdown and docker-compose syntaxes.
- Add docker volumes symblink.
- Add Traefik disclamer in docker-compose file.

### Changed

- Change always restart to unless-stopped.

### Fixed

- Fix default GitLab config with reverse proxy.
- Fix README syntax.

## [0.3.0] 2019-05-27

### Added

- Add SSH port variable.

### Changed

- Use named volumes.

## [0.2.0] 2018-12-06

### Added

- Add a GitLab Runner.

## [0.1.0] 2018-04-10

### Added

- Docker-compose setup for starting GitLab with Træfik.

[2.0.0]: https://github.com/solution-libre/docker-bareos/compare/v1.1.0...v2.0.0
[1.1.0]: https://github.com/solution-libre/docker-bareos/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/solution-libre/docker-bareos/compare/v0.3.0...v1.0.0
[0.3.0]: https://github.com/solution-libre/docker-bareos/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/solution-libre/docker-bareos/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/solution-libre/docker-bareos/releases/tag/v0.1.0
