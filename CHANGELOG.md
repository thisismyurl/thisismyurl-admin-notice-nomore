# Changelog

All notable changes to **Admin Notice NoMore by thisismyurl.com** are documented here.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the
project uses the `x.Yddd` versioning scheme: `x` = release class (`0` = pre-release,
`1` = full), `Y` = last digit of the year, `ddd` = Julian day.

## [1.6143] — 2026-05-23

### Changed
- Updated `Tested up to` to WordPress 7.0.
- Standardized the donation link to GitHub Sponsors (`https://github.com/sponsors/thisismyurl`).

### Added
- Project governance files: `PILLARS.md`, `CONTRIBUTING.md`, `SECURITY.md`, and README badges.

## [1.6140] — 2026-05-20

### Changed
- Updated display name to This Is My URL Admin Notice NoMore.
- Version moved to the `x.Yddd` Julian-day scheme.

### Added
- Nonce-protected one-request bypass URLs.
- Quick bypass shortcuts in plugin action links and the admin bar.

## [1.0.1]

### Added
- Emergency bypass for administrators via query parameter.
- Constants and filters for enable, bypass, and auto-dismiss control.

### Changed
- Switched auto-dismiss to opt-in by default.
- Scoped CSS selectors to notice contexts in `#wpbody-content`.

## [1.0.0]

### Added
- Initial release: global removal of admin-notice hooks, a CSS fallback for directly printed markup, and opt-in JavaScript auto-dismiss.
