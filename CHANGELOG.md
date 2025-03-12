# Action Stars Build Workflows for GitHub Actions Changelog

<!-- markdownlint-disable-next-line MD052 -->
> [!NOTE]
> All notable changes to this project will be documented in this file; the format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!--
### Added - For new features.
### Changed - For changes in existing functionality.
### Deprecated - For soon-to-be removed features.
### Removed - For now removed features.
### Fixed - For any bug fixes.
### Security - In case of vulnerabilities.
-->

## [UNRELEASED]

### Changed

- Updated _actions/attest-build-provenance_ from `2.2.2` to [`2.2.3`](https://github.com/actions/attest-build-provenance/releases/tag/v2.2.2). ([#4](https://github.com/action-stars/build-workflows/pull/4)) _@dependabot_

### Fixed

- Fix missing permission for validate job. ([#6](https://github.com/action-stars/helm-workflows/pull/6)) _@stevehipwell_

## [v0.2.0] - 2025-03-12

### Fixed

- Fix the image media type created by the _Build OCI Image_ workflow not being OCI. ([#5](https://github.com/action-stars/helm-workflows/pull/5)) _@stevehipwell_
- Fix missing annotation for the OCI image index created by the _Build OCI Image_ workflow. ([#5](https://github.com/action-stars/helm-workflows/pull/5)) _@stevehipwell_

## [v0.1.0] - 2025-03-12

### Added

- Add initial version of the _Build OCI Image_ workflow. ([#2](https://github.com/action-stars/helm-workflows/pull/2)) _@stevehipwell_

<!--
RELEASES
-->
[UNRELEASED]: https://github.com/action-stars/build-workflows/compare/v0.2.0...HEAD
[v0.2.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.2.0
[v0.1.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.1.0
