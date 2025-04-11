# Rem's Adventures - Project Structure

This document provides an overview of the project's structure and organization.

## Main Components

### Objects

The game uses various objects to implement gameplay mechanics:

- **obj_player**: The main player character with collision detection, movement controls, and state management
- **obj_game**: Core game logic including pause functionality, room management, and score tracking
- **Enemy Objects**:
  - **obj_bat_enemy**: Flying enemies that follow predefined paths
  - **obj_bird_enemy**: More complex enemies that can detect and chase the player
  - **obj_enemy1, obj_enemy2, obj_enemy3**: Various ground-based enemies with different behaviors
- **Environment Objects**:
  - **obj_block**: Solid platforms for the player to stand on
  - **obj_ground**: Base ground objects
  - **obj_spike**: Hazards that damage the player
- **Collectibles**:
  - **obj_coin**: Basic collectibles that increase score
  - **obj_blueorb, obj_yelloworb**: Special orbs with unique effects
- **UI Objects**:
  - Various button objects for menu navigation
  - **obj_menu, obj_gameover_menu**: Menu screens

### Rooms

The game is organized into different rooms:

- **rm_menu**: Main menu
- **rm_tutorial**: Tutorial level
- **rm_level1, rm_level2, rm_level3, rm_level4**: Main game levels
- **rm_pause_menu**: Pause screen
- **rm_game_over**: Game over screen
- **rm_credits, rm_story**: Additional information screens

### Resources

- **Sprites**: Visual assets for all game elements
- **Sounds**: Music and sound effects
- **Paths**: Predefined movement paths for enemies
- **Tilesets**: Themed tile collections for level design

## Code Organization

The game uses GameMaker Studio's event-based programming model:

- **Create Events**: Initialize objects and variables
- **Step Events**: Handle game logic that occurs each frame
- **Collision Events**: Handle interactions between objects
- **Draw Events**: Custom rendering for objects
- **Alarm Events**: Timed events for delayed actions

## Game States

The game manages different states:

- Normal gameplay
- Paused state
- Game over state
- Menu navigation

## Player States

The player can be in different states:

- Normal (right-side up)
- Upside down (gravity reversed)