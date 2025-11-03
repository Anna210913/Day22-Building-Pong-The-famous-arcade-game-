# Day 22: Building Pong! (The Famous Arcade Game)

Today, I built **Pong**, one of the first arcade video games ever created!
Fun fact: Pong was developed by **Allan Alcorn**, who had just joined the Atari company as a new engineer. The game wasn't even meant to be a real product rather it began as a *test project* assigned to him so that the company could evaluate his skills. Little did they know that this “simple challenge” would turn into a global hit, with Pong machines popping up in bars and arcades all over the world.

Programming something with such cool history reminds me just how versatile code truly is. Yes programming powers websites, apps, finance systems, and data tools, but it can also bring fun, interactive worlds to life.

How wild is it that I can sit here and write code that behaves like a real arcade machine from the 1970s?

# What I Learned:

- Setting up the game screen with `turtle` graphics  
- Creating paddle objects and responding to user key presses  
- Building multiple classes to organize game logic (`Paddle`, `Ball`, `Scoreboard`)  
- Animating the ball and controlling its movement  
- Detecting collisions with walls and paddles  
- Handling out-of-bounds logic and resetting positions  
- Implementing score tracking  
- Increasing ball speed (difficulty level) each time a point is scored

# How the Code Works
We used **Python Turtle** to build everything inside a basic window.

### The Paddles:
- Two paddles were created using a custom `Paddle` class
- Key bindings allow the left and right players to move their paddles up/down
- Movement uses `sety()` to adjust position smoothly

### The Ball:
- A `Ball` class controls movement and speed
- The ball moves continuously using `move()` and updates its direction on collisions
- Ball detects contact with the top/bottom walls → **bounces vertically**
- Ball detects collision with paddles → **bounces horizontally**
- If the ball passes a paddle, a point is awarded and the ball resets

### The Scoreboard:
- A `Scoreboard` class displays and updates the score for both sides
- Score increases when the opponent misses the ball

### Setting the Difficulty Feature:
- Every time a paddle scores, the ball speeds up
- Creates a fun and challenging gameplay progression just like the real game

