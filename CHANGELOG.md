# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.3.0] - 2026-09-06

### Added
- 4 new tracked categories, each with all 4 platform links: Coast Guard aircraft (458), drones/UAS (262), VIP & government transport (289), and worldwide aerial firefighting (356) — sourced from [`sdr-enthusiasts/plane-alert-db`](https://github.com/sdr-enthusiasts/plane-alert-db), a community-maintained, ODbL-licensed database (same license as this repo).
- A "Contents" section at the top of the README linking the main sections.
- A "Credits" section attributing the new categories' data source.

## [3.2.0] - 2026-09-06

### Added
- "Database Flag Filters" table documenting `filterDbFlag=` (military / PIA / LADD, live across the whole fleet, no curated ICAO list required).
- "Altitude, Range & Callsign Filters" table documenting `filterAltMin=`, `filterAltMax=`, `filterCallSign=`, and `filterMaxRange=`.
- "Build your own category link" how-to section explaining the `icao=` link pattern so contributors can construct and submit new categories.
- All new filter parameters verified against the upstream [`wiedehopf/tar1090` query-parameter reference](https://github.com/wiedehopf/tar1090/blob/master/README-query.md), the software every linked tracker runs on.

## [3.1.0] - 2026-09-06

### Fixed
- **Restored lost aircraft data**: the "Air Ambulances / Life Flights" and "Flights associated with the United Nations" rows had been silently overwritten with a duplicate of the "Law Enforcement Aircraft" ICAO list during the 2.0.0 reference-link rewrite. Recovered the original 808-aircraft Air Ambulances list and 24-aircraft UN list from project history and regenerated all four platform links for each.
- Removed 3 dead/duplicate reference-link definitions left over from the same rewrite.
- Fixed two Airplanes.live links pointing at `airplanes.live` instead of the working `globe.airplanes.live` pattern used everywhere else.
- Fixed table header mislabeling the Airplanes.live column as "ADSB.one".
- Deduplicated repeated ICAO codes in the LA/Palisades fires row.
- Fixed the "last commit" badge pointing at a stale repo name.
- Fixed two typos in the intro text.

## [3.0.0] - 2025-07-18

### Added
- Human-friendly project description explaining the purpose of curated airplane tracking links
- Comprehensive documentation of all ADSB tracking platforms
- Clear explanation of ICAO code filtering for focused aircraft tracking

## [2.0.0] - 2024-01-25

### Added
- Reference link system for easier maintenance and editing
- Support for four major ADSB tracking platforms (ADSBExchange, ADSB.lol, ADSB.fi, Airplanes.live)
- Comprehensive coverage of government, military, and law enforcement aircraft
- Sequential reference numbering system (1-48) for all tracking links
- Structured table format with Country, State, Description, and platform-specific links

### Changed
- **BREAKING**: Converted from inline links to reference link format
- Removed redundant "Link" text from column headers for cleaner presentation
- Improved table readability and maintenance workflow
- Enhanced aircraft categorization and descriptions

### Fixed
- All reference links properly defined and functional
- Consistent link formatting across all platforms
- Resolved file corruption issues with duplicate reference links
- Fixed missing and malformed reference definitions

## [1.0.0] - 2023-05-04

### Added
- Initial airplane spotting link collection
- Basic table structure for aircraft tracking
- LICENSE file with appropriate open source licensing
- Human-Readable-ODbl-Summary for licensing clarity
- Basic README.md documentation

### Changed
- Multiple iterative improvements to link accuracy and coverage
- Enhanced aircraft descriptions and categorization
- Improved geographic coverage and organization

### Fixed
- Various link corrections and updates
- Formatting improvements for better readability
- Licensing clarifications and updates

## [0.1.0] - Initial Release

### Added
- Initial commit with basic project structure
- Core concept of curated airplane tracking links
- Foundation for community-driven aircraft spotting resource

---

## Version History Summary

- **v2.0.0**: Major restructure with reference links, multi-platform support, and improved maintenance
- **v1.0.0**: Established stable link collection with comprehensive aircraft coverage
- **v0.1.0**: Initial project creation and concept development

## Technical Notes

- All links use ICAO code filtering for precise aircraft tracking
- Reference links are sequentially numbered for easy maintenance
- Four major ADSB platforms supported for comprehensive coverage
- Markdown reference link format enables easier editing and version control
