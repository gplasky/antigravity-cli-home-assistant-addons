# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-07-31
### Fixed
- Fixed Home Assistant sidebar panel icon configuration and metadata handling (`panel_icon: "mdi:terminal"`, `panel_admin: false`, proper YAML string quoting, and version bump to force Supervisor panel cache refresh).

## [1.0.9] - 2026-07-30
### Fixed
- Fixed an embarrassing bug where the sidebar panel icon was blank because `mdi:terminal` is not a valid Material Design Icon (the correct icon is actually `mdi:console`).

## [1.0.8] - 2026-07-30
### Fixed
- Restored the required `slug` parameter in `config.yaml` after build failure.

## [1.0.7] - 2026-07-30
### Fixed
- Fixed an issue where the Home Assistant frontend failed to render the sidebar panel icon due to explicit slug naming and quotes in `config.yaml`.

## [1.0.6] - 2026-07-30
### Fixed
- Fixed the missing sidebar icon by changing it to `mdi:terminal`, as `mdi:console` was not supported in all Home Assistant instances.

## [1.0.5] - 2026-07-30
### Changed
- Migrated GitHub Actions CI/CD to modern Home Assistant composite actions.
- Switched to Generic Manifest Image multi-arch publishing to natively support caching and speed up Home Assistant installation.

## [1.0.4] - 2026-07-30
### Fixed
- Fixed an issue where Home Assistant was building the add-on locally on the host machine instead of downloading the pre-built Docker container by correctly appending `-{arch}` to the image config.

## [1.0.3] - 2026-07-30
### Fixed
- Fixed an issue where the Home Assistant sidebar icon would fail to render by switching to a more broadly compatible `mdi:console` icon.

## [1.0.2] - 2026-07-30
### Fixed
- Fixed an issue where the legacy Gemini Spark image was still displaying in the Home Assistant Add-on README.

## [1.0.1] - 2026-07-30
### Changed
- Replaced the Gemini Spark logo and icon to better align with the new Antigravity branding.
- Changed the Home Assistant sidebar icon to a rocket (`mdi:rocket-launch`).
- Optimized `aarch64` build times by minimizing QEMU overhead.

## [1.0.0] - 2026-07-29
### Added
- Initial release of the standalone **Antigravity CLI** add-on for Home Assistant.
- Integrated `ha-mcp` server for deep smart home context.
- Persistent `tmux` terminal environment for long-running sessions.
