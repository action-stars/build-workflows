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

- Update _github/codeql-action_ from `3.28.16` to [`3.28.17`](https://github.com/github/codeql-action/releases/tag/v3.28.17). ([#14](https://github.com/action-stars/build-workflows/pull/14)) _@dependabot_

## [v0.5.0] - 2025-04-30

### Changed

- Update _github/codeql-action_ from `3.28.13` to [`3.28.14`](https://github.com/github/codeql-action/releases/tag/v3.28.14). ([#11](https://github.com/action-stars/build-workflows/pull/11)) _@dependabot_
- Update _github/codeql-action_ from `3.28.14` to [`3.28.15`](https://github.com/github/codeql-action/releases/tag/v3.28.15). ([#12](https://github.com/action-stars/build-workflows/pull/12)) _@dependabot_
- Update _github/codeql-action_ from `3.28.15` to [`3.28.16`](https://github.com/github/codeql-action/releases/tag/v3.28.16). ([#13](https://github.com/action-stars/build-workflows/pull/13)) _@dependabot_
- Update _actions/download-artifact_ from `4.2.1` to [`4.3.0`](https://github.com/actions/download-artifact/releases/tag/v4.3.0). ([#13](https://github.com/action-stars/build-workflows/pull/13)) _@dependabot_
- Update _docker/build-push-action_ from `6.15.0` to [`6.16.0`](https://github.com/docker/build-push-action/releases/tag/v6.16.0). ([#13](https://github.com/action-stars/build-workflows/pull/13)) _@dependabot_
- Update _actions/attest-build-provenance_ from `2.2.3` to [`2.3.0`](https://github.com/actions/attest-build-provenance/releases/tag/v2.3.0). ([#13](https://github.com/action-stars/build-workflows/pull/13)) _@dependabot_
- Update _sigstore/cosign-installer_ from `3.8.1` to [`3.8.2`](https://github.com/sigstore/cosign-installer/releases/tag/v3.8.2). ([#13](https://github.com/action-stars/build-workflows/pull/13)) _@dependabot_

## [v0.4.0] - 2025-03-27

### Added

- Add `WORKFLOW_ARTIFACTS` build argument to support accessing the artifacts passed to the workflow. ([#7](https://github.com/action-stars/helm-workflows/pull/7)) _@stevehipwell_

### Changed

- Only setup QEMU if the platform doesn't match the runner architecture. ([#7](https://github.com/action-stars/helm-workflows/pull/7)) _@stevehipwell_
- Update _docker/login-action_ from `3.3.0` to [`3.4.0`](https://github.com/docker/login-action/releases/tag/v3.4.0). ([#8](https://github.com/action-stars/build-workflows/pull/8)) _@dependabot_
- Update _github/codeql-action_ from `3.28.11` to [`3.28.13`](https://github.com/github/codeql-action/releases/tag/v3.28.13). ([#9](https://github.com/action-stars/build-workflows/pull/9)) _@dependabot_
- Update _actions/upload-artifact_ from `4.6.1` to [`4.6.2`](https://github.com/actions/upload-artifact/releases/tag/v4.6.2). ([#9](https://github.com/action-stars/build-workflows/pull/9)) _@dependabot_
- Update _actions/download-artifact_ from `4.1.9` to [`4.2.1`](https://github.com/actions/download-artifact/releases/tag/v4.2.1). ([#9](https://github.com/action-stars/build-workflows/pull/9)) _@dependabot_

## [v0.3.0] - 2025-03-12

### Changed

- Update _actions/attest-build-provenance_ from `2.2.2` to [`2.2.3`](https://github.com/actions/attest-build-provenance/releases/tag/v2.2.2). ([#4](https://github.com/action-stars/build-workflows/pull/4)) _@dependabot_

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
[UNRELEASED]: https://github.com/action-stars/build-workflows/compare/v0.5.0...HEAD
[v0.5.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.5.0
[v0.4.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.4.0
[v0.3.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.3.0
[v0.2.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.2.0
[v0.1.0]: https://github.com/action-stars/build-workflows/releases/tag/v0.1.0
