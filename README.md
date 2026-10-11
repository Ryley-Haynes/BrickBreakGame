# BrickBreakGame

A classic, interactive Brick Breaker game built for Android using Kotlin and the Android Canvas API.

## Features

- **Smooth Gameplay**: Real-time game loop driven by a dedicated timer task.
- **Touch Controls**: Intuitive paddle movement via touch and drag.
- **Scoring System**: Tracks your current score and persists your all-time best score using `SharedPreferences`.
- **Game States**: Includes a fully functional Pause/Resume menu and a Game Over screen with a restart option.
- **Sound Effects**: Audio feedback when the ball hits the paddle.
- **Dynamic Visuals**: Multi-colored bricks arranged in a grid that react to ball collisions.

## Project Structure

- **`MainActivity.kt`**: The entry point of the application, managing lifecycle events, touch input, and the game loop.
- **`BrickBreaker.kt`**: The core game engine handling physics, collision detection, scoring, and brick management.
- **`GameView.kt`**: Custom view responsible for rendering the game elements (ball, paddle, bricks) and the UI overlays.
- **`GameTimerTask.kt`**: Manages the periodic updates to the game model and view.

## Tech Stack

- **Language**: Kotlin
- **Platform**: Android
- **UI**: Android Canvas & Custom Views
- **Persistence**: SharedPreferences (for High Scores)
- **Audio**: SoundPool API

## Getting Started

1. Clone the repository.
2. Open the project in **Android Studio**.
3. Sync the project with Gradle files.
4. Run the app on an Android Emulator or a physical device (Minimum SDK: 24).

## How to Play

1. Tap the screen to start the game.
2. Drag your finger across the screen to move the paddle and keep the ball in play.
3. Break all the bricks to increase your score.
4. If the ball drops below the paddle, the game is over.
5. Use the **Pause** button to halt the game and access the menu.
