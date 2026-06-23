# Admin Notice NoMore

[![WordPress](https://img.shields.io/badge/WordPress-6.0%2B-21759b.svg)](https://wordpress.org/) [![License](https://img.shields.io/badge/License-GPL--2.0--or--later-blue.svg)](LICENSE)

Suppresses admin notices across wp-admin, with safety controls for the cases where you need them back.

## What it does

- Removes all registered callbacks for WordPress notice hooks
- Hides any remaining notice UI with scoped admin-side CSS
- Offers an optional auto-dismiss mode for dismissible notices (off by default)

## Why it exists

Some dashboards drown in plugin and update notices. The noise wears people down and makes the admin harder to work in. This plugin gives you one blunt option: turn the notices off. It is meant for teams that already handle updates, alerts, and security checks outside the dashboard, so the notices were never doing the job anyway.

## Requirements

- WordPress 6.0+
- PHP 7.4+

## Installation

1. Copy the plugin to `wp-content/plugins/thisismyurl-admin-notice-nomore`.
2. Activate Admin Notice NoMore from the Plugins screen.
3. Reload your wp-admin pages.

## Scope and trade-offs

This plugin is all-or-nothing by design, and that has real costs:

- It runs in wp-admin only.
- It hides every admin notice, including high-priority update and security nags.
- It can mask helpful guidance from plugins that lean on notice-based prompts.

Test it in staging first. Only move it to production once you are sure your update and security process does not depend on anyone seeing notices in the dashboard.

## Safety controls

- **Emergency bypass for administrators:** add `?thisismyurl_nomore_show_notices=1` to any admin URL to see notices again for that request
- **Constant toggle:** `THISISMYURL_ADMIN_NOTICE_NOMORE_ENABLED`
- **Constant bypass:** `THISISMYURL_ADMIN_NOTICE_NOMORE_BYPASS`
- **Optional JS auto-dismiss:** `THISISMYURL_ADMIN_NOTICE_NOMORE_AUTO_DISMISS`
- **Filters:** `thisismyurl_admin_notice_nomore_enabled`, `thisismyurl_admin_notice_nomore_bypass`, `thisismyurl_admin_notice_nomore_auto_dismiss`, `thisismyurl_admin_notice_nomore_css_selectors`

## Versioning

Versions follow `X.Yjjj.hhmm` — year, Julian day, 24-hour time of the build.

## About

Admin Notice NoMore is built and maintained by [Christopher Ross](https://thisismyurl.com/). I build focused WordPress tools for problems that keep showing up across real sites. No tracking, no ads, no upsells.

**WordPress.org:** [profiles.wordpress.org/thisismyurl](https://profiles.wordpress.org/thisismyurl/) · **GitHub:** [github.com/thisismyurl](https://github.com/thisismyurl) · **LinkedIn:** [linkedin.com/in/thisismyurl](https://linkedin.com/in/thisismyurl)

## License

GPL-2.0-or-later. See [LICENSE](LICENSE).
