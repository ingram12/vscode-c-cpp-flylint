# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]
### Added

### Changed
- Display an informational message when a given analyzer is unable to
  activate due to missing binary or configuration file.
- Improve generic error message: added a note to check the console
  output.

## [0.1.0] - 2017-06-19
### Added
- Added a command to force the analysis of the current document.
- Added a command to force the analysis of all opened documents within the
  workspace.
- A change log to quickly view an overview of the changes made to each version
  of the extension.
- Added flag to enable verbose debug logging. This was previously the default
  mode of operation.
- Refactored the most typical options, common between analyzers, to a common
  base configuration set. The base configuration set will cascade to all
  analyzers, by default.

### Changed
- Fixed duplicate analyzers being ran after configuration change.
- Redefined how the `c-cpp-flylint.run` configuration option functions.
- Always ensure a starting column is selected, even if RegExp fails.

## [0.0.1] - 2017-06-18
- Initial release.