Here’s a simple README file for the **Flappy Bird** game implemented in Java:

```markdown
# Flappy Bird in Java

A simple **Flappy Bird** clone created in Java using the `javax.swing` library. The game is controlled using the spacebar, and the goal is to navigate the bird through an infinite series of pipes without crashing into them.

## Features

- **Bird Flapping Physics**: The bird moves up when the spacebar is pressed and falls down due to gravity.
- **Pipe Generation**: Pipes are generated randomly at different vertical positions with a gap in between.
- **Score Calculation**: The score increments each time the bird successfully passes through a pair of pipes.
- **Collision Detection**: The game detects collisions between the bird and pipes, and ends when a collision is detected or the bird falls out of the screen.
- **Game Over**: When the game is over, the final score is displayed and the game can be restarted by pressing the spacebar.

## Installation

To run this project, you need to have **Java** installed on your system.

1. Clone the repository:

   ```bash
   git clone https://github.com/SarangChauhan246/Flappy_Bird
   ```

2. Compile and run the `FlappyBird.java` file:

   ```bash
   javac FlappyBird.java
   java FlappyBird
   ```

## Controls

- Press `Spacebar` to make the bird flap its wings.
- If the bird collides with a pipe or falls off the screen, the game will end.
- Press `Spacebar` again to restart the game after a game over.

## Game Logic

- **Bird Movement**: The bird has an initial velocity of `0` and is constantly affected by gravity (`+1` to `velocityY`). When the spacebar is pressed, the bird's vertical velocity is set to `-9`, which causes it to "jump".
- **Pipe Movement**: Pipes move leftward across the screen with a constant horizontal velocity (`-4` units). New pipes are added every 1.5 seconds, and the game maintains a gap between the top and bottom pipes.
- **Collision Detection**: A simple Axis-Aligned Bounding Box (AABB) collision detection method is used to determine if the bird hits a pipe or if it flies out of bounds.
- **Scoring**: The score is incremented by `1` each time the bird successfully passes a pair of pipes.



## Requirements

- **Java Development Kit (JDK)** version 8 or higher
- **Swing** and **AWT** libraries (included with Java)

## Code Structure

- **FlappyBird.java**: The main class that handles the game's rendering, logic, and event handling.
- **Bird Class**: Manages the bird’s position, size, and image.
- **Pipe Class**: Manages the position, size, and image of the pipes.



## License

This project is open-source and available under the **MIT License**.

