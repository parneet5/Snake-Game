# Snake-Game

This project is a terminal-based implementation of the classic Snake Game written in C. 
It features smooth, real-time gameplay entirely within the console window and supports dynamic snake movement, fruit collection, score tracking, and collision detection with the tail. 
The game runs on both Linux and macOS terminals (and potentially Windows with a suitable terminal emulator) using non-blocking input and low-level terminal handling.
The game area is drawn as a bordered grid where the snake (O) moves around to eat randomly spawned fruits (F). 
Every time the snake eats a fruit, its tail grows longer, and the score increases by 10. 
If the snake collides with its own tail, the game ends with a “Game Over” message. 
The snake wraps around screen edges instead of dying, making gameplay more forgiving but still challenging.
Real-time input is handled using termios to disable input buffering and echo, allowing the snake to move immediately upon key presses (WASD controls). 
The screen refreshes at a speed that scales with the score, making the game faster as the player progresses. 
Terminal manipulation, input detection using select(), and dynamic tail rendering make this game a fun and engaging console experience.
This project demonstrates skills in system-level programming, handling terminal input/output, game loop design, and real-time interaction in C—all without external libraries.
