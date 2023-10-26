# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

The changelog is applicable from version `1.0.0` onwards.

---

## [Unreleased] - YYYY-MM-DD

### Added

### Fixed

- APED-74: Fix memory issue causing NiFi to crash.
- APED-66: Fix tag bug workaround in `publish.yml` workflow.

### Changed

[Commits](https://github.com/brightsparklabs/nifi-provenance-reporting-bundle/compare/2.1.0...develop)

## [2.1.0] - 2023-09-19

### Added

- APED-33: Added Changelog Enforcer.
- APED-44: Add attribute inclusion and exclusion lists for output to Elasticsearch.

### Changed

- APED-34: Updated README.
- APED-43: Set default run schedule for `ElasticsearchProvenanceReporter` to `"1 min"`.

[Commits](https://github.com/brightsparklabs/nifi-provenance-reporting-bundle/compare/2.0.0...2.1.0)

---

## [2.0.0] - 2023-07-04

### Added

- APED-18: Migrate to Java 17 and latest NiFi.
- APED-20: Added gradle-baseline support.
- APED-23: Support dependabot updates.

[Commits](https://github.com/brightsparklabs/nifi-provenance-reporting-bundle/compare/1.0.0...2.0.0)

---

## [1.0.0] - 2023-07-03

### Added

- APED-15: Added mutual TLS support for connecting to Elasticsearch.
- APED-19: Support overriding properties via environment variables.
- APED-24: Support publishing to Maven Central for posterity.

### Changed

- APED-14: Dependency updates.
- APED-16: Migrated from maven to gradle.

---

# Template

## [Unreleased] - YYYY-MM-DD

### Added

### Fixed

### Changed

[Commits](https://github.com/brightsparklabs/nifi-provenance-reporting-bundle/compare/2.0.0...)

---
