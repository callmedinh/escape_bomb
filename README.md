# EscapeBoom

A 2D multiplayer game where players try to avoid holding the bomb for too long!

## Game Rules

- At the start, 4 players are spawned in the scene.
- A random player is assigned the "Boom" (bomb).
- The player holding the Boom has a 10-second timer.
- If the timer reaches 0 while holding the Boom, the player explodes and loses.
- If a player collides with another player, the Boom is instantly transferred to the collided player and the timer resets.
- After a player explodes, they are removed from the game.
- The game continues until only one player remains. The last player wins.

## Game Components

### PlayerController
- Handles player movement and collision detection.
- Manages the visual representation of the bomb.
- Implements AI behavior for bot players.

### BombManager
- Manages who holds the bomb and the timer logic.
- Handles bomb transfer between players.
- Updates the UI to show the timer and bomb holder.

### GameManager
- Controls the game flow (start, playing, game over).
- Manages win/lose conditions.
- Coordinates between PlayerManager and BombManager.

### PlayerManager
- Handles player spawning and removal.
- Manages player colors and AI settings.

### UIManager
- Controls the game UI (main menu, gameplay, game over).
- Updates the timer display.
- Shows the winner when the game ends.

## Customization

You can customize the game by modifying the following parameters:

- Number of players (in PlayerManager)
- Bomb timer duration (in BombManager)
- Player colors (in PlayerManager)
- AI behavior (in PlayerController)
- UI layout and appearance (in UIManager)
