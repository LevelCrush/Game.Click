# Clicker Game Project

## Overview
This is an interactive single-page web application that combines clicking mechanics with dynamic visual effects, random YouTube video integration, and engaging mini-games.

## Features

### Core Gameplay
- **Click Counter**: Large centered number that increments with each click/tap
- **Bonus System**: Earn extra clicks by performing well in mini-games

### YouTube Integration
- **Random Video Playback**: 10% chance per click to trigger a video
- **Curated Library**: 40+ handpicked entertaining videos
- **Smart Selection**: No repeat videos back-to-back
- **Auto-play After Games**: New video starts when mini-game ends
- **Seamless Experience**: Videos play in background with full audio

### Mini-Games
Four different mini-games that appear dynamically:
1. **Whack-a-Mole**: Click moles as they pop up from holes
2. **Bubble Pop**: Pop bubbles floating up the screen
3. **Target Practice**: Shoot moving targets with accuracy-based scoring
4. **Points of Interest**: Click colorful shapes for varying points (1-5 points based on shape)

### Mini-Game System
- **Dynamic Scheduling**: Games appear every 20-30 seconds based on click rate
- **Adaptive Frequency**: Faster clickers see more mini-games
- **No Repeats**: Different game each time
- **10-Second Timer**: Quick, engaging gameplay
- **Bonus Rewards**: Earn clicks equal to 50% of your game score

### Visual Effects
- **Particle Explosions**: Colorful particles burst at click locations
- **Ripple Effects**: Expanding circles on each click
- **Dynamic Gradients**: Background colors follow mouse movement
- **Random Color Flashes**: 30% chance for background flash on click
- **Layered Z-Index**: Effects properly layer over all elements

### Animations
- **Bounce Effect**: Counter scales on each click
- **Smooth Transitions**: All UI elements animate smoothly
- **Shape Animations**: Mini-game objects have unique animations (pulse, spin, wobble)
- **Particle Physics**: Realistic explosion trajectories

## Technical Details
- **Pure Vanilla Stack**: HTML/CSS/JavaScript (no external dependencies)
- **YouTube IFrame API**: Proper video lifecycle management
- **CSS Animations**: Hardware-accelerated effects
- **Click Rate Tracking**: Monitors user interaction patterns
- **Responsive Design**: Works on all screen sizes
- **Event-Driven Architecture**: Clean separation of concerns

## Performance Features
- **Automatic Cleanup**: Particles and effects self-remove
- **Optimized Animations**: Using CSS transforms for smooth 60fps
- **Smart Scheduling**: Mini-games based on actual click rate
- **Memory Management**: Proper cleanup of video players and game elements

## File Structure
- `index.html` - Single page application containing all code
- `CHANGELOG.md` - Detailed version history
- `CLAUDE.md` - This technical documentation
- `README.md` - User-facing documentation

## Usage
Simply open `index.html` in any modern web browser and start clicking!

## Development Notes
- Mini-games use z-index 100+ to appear above videos
- Videos use z-index 1, counter uses z-index 10
- Click tracking window: 30 seconds for rate calculation
- Minimum 10 clicks required between games
- All timers and intervals properly cleaned up