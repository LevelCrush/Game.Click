# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Fixed
- Users can now continue clicking while YouTube videos are playing
  - Lowered YouTube container z-index to stay below counter
  - Added pointer-events: none to iframe element
  - Removed click blocking during video playback
- Fixed particle effects z-index to ensure they appear above other elements
  - Set z-index: 20 for both particle and ripple elements
  - Ensures visual effects are not hidden behind YouTube container
- Improved YouTube video timing accuracy
  - Implemented YouTube IFrame API for precise video end detection
  - Replaced timeout-based approach with event-driven video state tracking
  - Added proper error handling for failed video loads
  - Videos now fade out exactly when they finish playing

## [1.0.0] - 2025-01-06

### Added
- Initial release of the clicker game
- Click counter with bounce animations
- Random YouTube video integration (10% chance per click)
- Particle explosion effects at click locations
- Dynamic gradient backgrounds that follow mouse movement
- Ripple effects on clicks
- Random background color flashes
- Responsive single-page design
- Project documentation (CLAUDE.md)