# Changelog
This file contains all the notable changes done to the Ballerina Microsoft Dynamics 365 Finance and Operations package through the releases.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed
- Removed the placeholder default value (`https://your-org.operations.dynamics.com/data`) from the `serviceUrl` parameter of every connector's `init` function, across all 30 packages. `serviceUrl` is now a required parameter, so client initialization no longer silently targets a non-existent organization when the URL is omitted. The expected URL structure is now documented in the `init` docstring.
- Reworded each package's README overview line to drop the fully-qualified module name (e.g. "The `microsoft.dynamics365.finance.coreorg` connector provides access..." is now "The connector provides access...").

## [0.2.0]

### Changed
- Expanded the connector surface to ~300 entity sets with list / get / create / update / delete operations.
- Operation names and field names changed vs 0.1.0; consumers depending on 0.1.0 should pin that version explicitly.

## [0.1.0] - 2026-04-22

### Added
- Initial implementation of the Microsoft Dynamics 365 Finance and Operations connector.
