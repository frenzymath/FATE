# Changelog

## [1.2.0] - 2026-02-23

### Added
- Added support for all Lean minor versions from [v4.19.0] through [v4.28.0].

## [1.1.0] - 2026-02-23

### Added
- This CHANGELOG file and CHANGELOG files for FATE-M, H and X.
- Added an entry to the JSON files recording the compatible Lean version.
- The JSON file in FATE-X now contains an entry for new declarations introduced in each benchmark problem.
- Added imports for all files to the root file in FATE-X to ensure CI works.

### Fixed
- Resolved misalignments between formal and natural language statements in the following problems:
  - **M-15**
  - **M-134**
- **H-93**: The `CancelCommMonoidWithZero` instance on `Ideal R` resulted in a diamond in the monoid structure. Moreover, there was a subtle semantic distinction between `UniqueFactorizationMonoid (Ideal O)` and the unique factorization of ideals: a nonzero prime ideal is not necessarily a prime element in the monoid of ideals *a priori*, without knowing the ring is a Dedekind domain. The problem now directly expresses the existence and uniqueness of ideal decomposition.
- **X-11**: Fixed reversed order of parameters in `MvPolynomial`.
- **X-77**: Added missing Noetherian condition.
- **X-86**: Fixed reversed order of parameters in `MvPolynomial`.

### Changed
- Removed void references from the informal statements of M-79 and M-150. The formal statements are unaffected.
- **H-12**: Changed the notation $<$ to $\le$ in the natural language statement to cover the case H = G. The formal statement is unaffected.
- **X-54**: Updated the informal statement and comments to align with the formal statement. The formal statement is unaffected.
- Added a unique namespace to each problem in FATE-X to avoid conflicts from repeated definitions in CI.
- Corrected minor formatting issues in comments and standardized all comments to use `/-- ... -/`.

## [1.0.1] - 2025-09-22

### Fixed
- Fixed shifted domain tags in the JSON files for FATE-H and FATE-X.
- Fixed the sunburst chart for domain statistics.

## [1.0.0] - 2025-08-26

### Added
- First release of the FATE benchmark series, consisting of FATE-M, FATE-H, and FATE-X. Each benchmark contains:
  - A PDF file with both natural language statements and their formalizations for human reading.
  - A JSON file for machine reading.
- Sunburst chart for domain statistics of FATE-H and FATE-X.

[v4.28.0]: https://github.com/frenzymath/FATE/tree/v4.28.0
[v4.19.0]: https://github.com/frenzymath/FATE/tree/v4.19.0
[1.1.0]: https://github.com/frenzymath/FATE/tree/40eff93d3fa8a06a73d67b28480d14bd28ec1c3c
[1.0.1]: https://github.com/frenzymath/FATE/tree/129a05ce00002a6c73f4a2ad032a23e6c7a51189
[1.0.0]: https://github.com/frenzymath/FATE/tree/initial-release
