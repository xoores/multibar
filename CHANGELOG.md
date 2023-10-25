# Changelog

All notable changes to this project will be documented in this file.
Each release should have the following subsections, if entries exist, in the
given order: `Breaking`, `Build`, `Deprecated`, `Removed`, `Added`, `Changed`,
`Fixed`, `Security`.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased 1.0.0]
### Added
- Hover actions ([Polybar PR #2868 by @Astrono2](https://github.com/polybar/polybar/pull/2868))
  - Support for actions on hover via action numbers `9` and `10` ([`Polybar #1064`](https://github.com/polybar/polybar/issues/1064), [`Polybar #2868`](https://github.com/polybar/polybar/pull/2868)).
  - `custom/script`: `hover-start` and `hover-end` actions ([`Polybar #1064`](https://github.com/polybar/polybar/issues/1064), [`Polybar #2868`](https://github.com/polybar/polybar/pull/2868)).
  - Added support for TAG_LABEL (`<label>`) in ipc module  ([`Polybar #2841`](https://github.com/polybar/polybar/pull/2841))  by [@madhavpcm](https://github.com/madhavpcm).
  - Added support for format-i for each hook-i defined in ipc module ([`Polybar #2775`](https://github.com/polybar/polybar/issues/2775),  [`Polybar #2810`](https://github.com/polybar/polybar/pull/2810))  by [@madhavpcm](https://github.com/madhavpcm).
- Network unit type ([Polybar PR #3001 by @Cationiz3r](https://github.com/polybar/polybar/pull/3001))
  - `internal/network`: `metric-units` setting
- reverse-scroll, logarithmic-scroll and click-toggle ([Polybar PR #2703 by me](https://github.com/polybar/polybar/pull/2703))
  - `internal/backlight`:
    - Added `reverse-scroll` option and LEFT_CLICK action
    - Added `scroll-log` option that enables logarithmic adjustment of brightness


[1.0.0]: https://github.com/xoores/multibar/
