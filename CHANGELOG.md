# Changelog

All notable changes to TaskbarAIMonitor will be documented in this file.

## [Unreleased]

## [0.1.7]

- Flyout update banner now links to the changelog (`changelog ↗`) for the
  pending version.

## [0.1.6]

- Refreshed bundled dependencies.

## [0.1.5]

- Flyout header now shows the app name and version instead of "AI usage".
- Flyout header shows the next scheduled refresh next to "updated";
  the footer's auto-refresh hint was removed.
- Flyout reset credits: expiration dates sit next to the "Reset credits"
  label, which now reads "Reset credits: N".

## [0.1.4]

- Settings gained a page header on every tab: the section title and
  description now sit on a dark band with an accent edge instead of a
  small inline heading.
- Fixed the "quota window has started over" toast firing on every Codex
  poll: an unused session window reports `reset_at` as request time plus the
  window length, so the timestamp drifted forward each fetch and looked like
  a rollover.
- The Codex reset-credit badge in the taskbar strip now shows only the
  days until the nearest credit expires — the credit count stays
  in the flyout.

## [0.1.3]

- Pending updates are now flagged in three places: a green `↑ version` pill
  at the end of the taskbar strip, an Install banner inside the flyout, and
  a matching dot painted onto the tray icon.

## [0.1.2]

- New "Remaining time" checkbox in Settings → Taskbar (on by default):
  shows a compact countdown to each quota window's reset — e.g. `3d`,
  `5h`, `47m` — to the left of every bar in the taskbar strip.
- Devin's exhausted daily/weekly quota now shows as 0% in the flyout instead
  of the row disappearing.
- Settings → DeepSeek now shows the key source explicitly: a `DEEPSEEK_API_KEY`
  row displays the masked env key (`sk-***`) or "(not set)", and the key field
  below is for a manually saved override.

## [0.1.1]

- Fixed "Start with Windows" not taking effect on fresh installs: the Run
  entry is now written during setup, removed on uninstall and kept in sync
  at every launch.

## [0.1.0]

- Initial release.
