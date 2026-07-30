# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
