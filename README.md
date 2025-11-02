# SnakeGame

🐍 Snake Game (Java Swing)
- A classic Snake Game built in Java using the Swing and AWT libraries.
- The player controls a snake that moves around the screen, eats apples to grow, and tries to avoid colliding with the walls or itself.

🎮 Features
- Responsive keyboard controls (arrow keys)
- Randomly spawning apples
- Dynamic snake growth with each apple eaten
- Real-time score display
- Collision detection and game over screen
- Simple and clean user interface built with JFrame and JPanel

🧩 Project Structure

- SnakeGamePackage/
     - GamePanel.java     # Handles the game logic, drawing, and keyboard controls
     - GameFrame.java     # Sets up the main window and adds the GamePanel
     -  SnakeGame.java     # Entry point; runs the game

⚙️ Requirements
- Java 17+ (or any version supporting Swing and AWT)
- A Java-compatible IDE (e.g., IntelliJ IDEA, Eclipse, or VS Code with Java extension)
- No external dependencies required

🚀 How to Run
- Clone or Download this repository.
- Open the project in your Java IDE or terminal.
- Ensure the folder structure looks like this:
    - src/
       -   SnakeGamePackage/
       -    SnakeGame.java
       -    GameFrame.java
       -    GamePanel.java
- Compile and Run:
  - javac SnakeGamePackage/*.java
  - java SnakeGamePackage.SnakeGame
  - The game window will open automatically.

🕹️ Controls

- Key	Action
- ⬆️	Move Up
- ⬇️	Move Down
- ⬅️	Move Left
- ➡️	Move Right

💡 Gameplay Rules
- The snake starts moving to the right by default.
- Every time the snake eats an apple, its body grows by 1 segment and the score increases by 1.
- The game ends when the snake:
  - Collides with its own body
  - Hits the walls of the screen
- The final score is displayed on the Game Over screen.

🧠 Code Overview
GamePanel.java
- Core logic of the game.
Handles:
- Drawing the grid, snake, and apples.
- Detecting collisions.
- Responding to keyboard input.
- Updating game state on each timer tick (ActionListener).
GameFrame.java
- Creates the game window using JFrame.
- Adds the GamePanel and sets up basic properties like title, size, and close behavior.
SnakeGame.java
- The main class that initializes and launches the game by creating a GameFrame.

🧰 Key Concepts Demonstrated
- Object-Oriented Design: Encapsulation using separate classes for frame, panel, and main logic.
- Swing Components: JFrame, JPanel, Timer, Graphics.
- Event Handling: Implements ActionListener and uses KeyAdapter for keyboard input.
- Game Loop Mechanics: Timer-driven updates to refresh the screen and manage motion.
