# Cubo Jump

Cubo Jump is a physics-based 2D platformer built from the ground up using the HTML5 Canvas API and Vanilla JavaScript. The project demonstrates advanced logic in physics simulation, momentum-based movement, and complex collision detection.

---

![img](https://github.com/Faraz-Ali-1/2D-Platformer-Game/blob/4ba235d9552dfc8abdc38a1d32bf1950c23b232b/screenshots/cubo%201.jpg)

---

## Live Demo

https://faraz-ali-1.github.io/2D-Platformer-Game/

---

## Technical Features

### Custom Physics Engine
Developed a robust physics system that simulates gravity, terminal velocity, and horizontal friction. This ensures that the cube’s movement feels organic rather than static, with smooth acceleration and deceleration curves.

### Object-Oriented Architecture (OOP)
Utilized JavaScript Constructors to create a scalable game environment. By using a class-based approach for the Player, Platforms, and Obstacles, the code remains DRY (Don't Repeat Yourself) and allows for the easy addition of new levels and entities.

### Collision Detection & Response
Implemented precise Axis-Aligned Bounding Box (AABB) collision algorithms. The system detects interactions on all four sides of the cube, preventing "clipping" through platforms and allowing for solid-object interaction with obstacles.

### Checkpoint & State Management
Integrated a checkpoint system that stores the player's progress. The game handles state changes to manage respawns, ensuring that reaching a checkpoint saves the coordinates for the player's next attempt.

---

![img](https://github.com/Faraz-Ali-1/2D-Platformer-Game/blob/4ba235d9552dfc8abdc38a1d32bf1950c23b232b/screenshots/cubo%202.jpg)

---

## Lessons Learned & Challenges

### The Challenge of "Perfect" Physics
One of the most difficult parts of development was preventing the cube from "jittering" when standing on a platform. I solved this by implementing a "velocity reset" and "position snapping" logic—once the player's bottom edge hits a platform, the downward velocity is set to zero and the Y-position is perfectly aligned with the platform surface.

### Coordinate Mapping on Canvas
Mapping the collision boxes to the visual pixels on the Canvas required deep knowledge of the coordinate system. I struggled initially with the "refresh" rate of the game loop, which I fixed by utilizing `requestAnimationFrame` to ensure smooth 60FPS performance across different monitor refresh rates.

---

## Tech Stack

* **Engine:** HTML5 Canvas API
* **Logic:** Vanilla JavaScript (ES6+)
* **Architecture:** Constructor-based OOP
* **Physics:** Custom Gravity & Collision Algorithms

---

![img](https://github.com/Faraz-Ali-1/2D-Platformer-Game/blob/4ba235d9552dfc8abdc38a1d32bf1950c23b232b/screenshots/cubo%203.jpg)

---

## Installation & Controls

1. Clone the repository to your local machine.
2. Open the `index.html` file in any modern web browser.

**Controls:**
* **Left/Right Arrows:** Move the Cube.
* **Space/Up Arrow:** Jump (Logic includes gravity calculation).

---

## License

This project is licensed under the MIT License.
