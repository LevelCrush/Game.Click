# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Added
- Mini-game system with 4 different games
  - Whack-a-Mole: Click moles as they pop up
  - Bubble Pop: Pop bubbles floating to the top
  - Target Practice: Shoot moving targets with accuracy-based scoring
  - Points of Interest: Click colorful shapes for varying points
- Dynamic mini-game scheduling based on click rate
  - Games appear every 20-30 seconds on average
  - Faster clicking leads to more frequent games
  - Minimum clicks required between games
- Mini-game features
  - 10-second timer for each game
  - Score system with bonus clicks reward (50% of score)
  - No repeat games back-to-back
  - Games display over YouTube videos (z-index: 100)
- YouTube video improvements
  - Expanded video library with 40+ curated videos
  - Automatic video playback after mini-games end
  - No repeat videos back-to-back
  - Seamless video switching functionality

### Changed
- Bubble float animation now reaches full viewport height
- Bubble animation duration increased from 4s to 8s
- Mini-game timing changed from 40-60s to 20-30s intervals

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