# Star Catcher: Interactive Canvas Physics

A lightweight, interactive 2D physics engine and game loop built entirely with Vanilla JavaScript and the HTML5 Canvas API. 

This project demonstrates core concepts of interactive web development, including continuous rendering loops, vector-based mathematics, collision detection, and dynamic state management without the use of external game engines or libraries.

## 🚀 Technical Architecture

The simulation is built around a custom game loop utilizing `requestAnimationFrame` for smooth 60fps rendering. It highlights several key technical competencies:

### 1. Vector Math & Trigonometry
* **Rotational Kinematics:** The player's ship dynamically tracks the cursor's position using the `Math.atan2()` function, allowing for fluid, continuous rotational alignment.
* **Velocity & Friction:** Movement is not mapped 1:1 to the mouse coordinates. Instead, the cursor acts as an attractor point. The ship accelerates towards it, while a constant damping factor (friction) is applied to its velocity vectors (`vx`, `vy`) to create a smooth, drifting flight mechanic.

### 2. Collision Detection
* **Distance Calculation:** The engine continuously calculates the distance between the ship's coordinates and the target (the star) using the Pythagorean theorem. If the threshold is crossed, a collision event is triggered.

### 3. Dynamic Particle System
* **Array Management:** Upon collision, the game instantiates a burst of particle objects. 
* **Garbage Collection:** Each particle is assigned a lifecycle (`life`). As the animation progresses, their opacity decreases. Once a particle's lifecycle reaches zero, it is dynamically spliced from the rendering array to prevent memory leaks and ensure optimal performance.

## 💻 Tech Stack
* **HTML5 Canvas:** For high-performance 2D rendering.
* **CSS3:** For modern, responsive layout and UI styling.
* **Vanilla JavaScript (ES6+):** Object-oriented principles and event-driven interaction handling.

## 🎮 How to Play
1. Move your mouse (or drag your finger on a touchscreen) across the canvas.
2. The ship will automatically rotate and thrust towards your cursor.
3. Collect the glowing stars to increase your score and trigger the particle effects.

---
*Created as part of a technical portfolio demonstrating interactive web design and foundational software engineering principles.*
