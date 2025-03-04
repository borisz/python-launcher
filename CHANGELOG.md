# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/) (because [Rust makes me](https://doc.rust-lang.org/cargo/reference/manifest.html#the-version-field), [not because I want to](https://snarky.ca/why-i-dont-like-semver/)).

## Unreleased

See the changelog fragments in the [`changelog.d` directory](https://github.com/brettcannon/python-launcher/tree/main/changelog.d).

<!-- scriv-insert-here -->

## 1.0.0 — 2021-07-24

### Added

- Release instructions to `CONTRIBUTING.md`.

### Added

- Documentation for `ExactVersion`'s fields.

### Changed

- Add a release step to check action workflows for success.

## 0.18.1 — 2021-07-24

### Fixed

- Changelog and release note generation as part of the release pipeline now works.

### Added

- All shell commands in the release pipeline now specify bash as the shell.

## 0.18.0 — 2021-07-24

### Added

- A changelog (powered by [scriv](https://scriv.readthedocs.io/) by @nedbat; [#122](https://github.com/brettcannon/python-launcher/issues/122)).

### Changed

- Moved all tests over to Rust (#126 and implicitly solves the same problem that #109 was meant for).

### Fixed

- When the current working directory is invalid (e.g. doesn't exist or insufficient permissions), don't trigger a panic (fixed as a side-effect of #125).

## 0.17.0 — 2021-07-18

### Changed

- Make malformed PY_PYTHON\* environment variables cause a launch failure while providing a better error message and documentation (#114; thanks @treyhunner , @jefftriplett for reviews).

## 0.16.0 — 2021-06-04

### Added

- Everything (initial release).
