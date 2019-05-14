# Changelog

## [0.8] - 2019-05-13
### Added
- `OrdAttMap` to create maps that preserve insertion order and otherwise behave like ordinary `AttMap`
- `get_data_lines` utility, supporting nice instance `repr`
- `is_custom_map` utility
### Changed
- Better `repr` and `str` for all `attmap`-like types, rendering like YAML
- `__getitem__` syntax on `AttMapEcho` no longer exhibits echo behavior (only dot notation does.)
- Instance comparison is now much stricter, requiring exact type match. This reflects some of the type-specific value conversion and representation behavior.
- `PathExAttMap` is now `OrdPathExAttMap`, preserving item insertion order
- `AttMapEcho` preserves item insertion order

## [0.7] - 2019-04-24
### Changed
- Removed `pandas` dependency
- Made hooks for omission of specific keys instance methods

## [0.6] - 2019-04-11
### Added
- Hook for omission of key(s) from instance comparison
- Documentation

## [0.5] - 2019-03-27
### Added
- Add `to_map` method to convert `Mapping` values to basic type

## [0.4] - 2019-03-19
### Changed
- What was `PepAttMap` is now `PathExAttMap`.

## [0.3] - 2019-03-19
### Added
- `PepAttMap` attempts expansion of text value as a path, using available environment variables
### Changed
- `AttMap` now derives from `PepAttMap` rather than ordinary `AttMap`

## [0.2] - 2019-03-04
### Changed
- `AttMapEcho` now converts an inserted `Mapping` to `AttMapEcho` -- no more specific type than that.
- Handle equivalence comparison when values are array-likes from `numpy` or `pandas`

## [0.1.8] - 2019-02-06
### Fixed
- Installation working for dependent packages

## [0.1.7] - 2019-02-05
### Changed
- Make `__version__` available on the main package object

##  [0.1.6] - 2019-02-05
### Changed
- Bound on most specific type to which a stored `Mapping` should be converted can be controlled in a subclass via overriding.

## [0.1.5] - 2019-02-05
### Changed
- `add_entries` method on an `AttMapLike` now returns the instance.
- Improve test coverage

## [0.1.4] - 2019-02-05
### Changed
- Removed support for Python 3.4

## [0.1.3] - 2019-02-05
### Fixed
- Pass unit tests on Python 3.4

## [0.1.2] - 2019-02-04
### Fixed
- Correct PyPI landing page rendering

## [0.1.1] - 2019-02-04
### Fixed
- Correct PyPI landing page rendering

## [0.1] - 2019-02-04
### New
- Initial release
