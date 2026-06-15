# Star Catcher 🚀

An elegant, interactive 2D space game built entirely from scratch using HTML5 Canvas and Vanilla JavaScript. Pilot your rocket through deep space and gather the stars!

## 🎮 Live Demo
**No setup or technical knowledge required!** You can launch and play the game instantly in your browser by clicking the link below:
👉 [**CLICK HERE TO PLAY THE GAME**](https://kristina-neureuther.github.io/star-catcher/)

---

## 🕹️ How to Play
1. Click the **Live Demo** link above to open the game.
2. Move your computer mouse (or drag your finger on a mobile touchscreen).
3. Your rocket will automatically rotate and smoothly glide toward your cursor.
4. Collect all **25 gold stars** scattered across the screen. Once they are all gone, you win!

## 💻 Technical Highlights (For Developers)
For those interested in the software architecture, this project demonstrates:
* **Interactive Physics:** Smooth object tracking utilizing velocity vectors, acceleration, and artificial friction (damping) for a realistic drifting feel in space.
* **Collision Detection:** Continuous real-time calculations using the Pythagorean theorem to detect when the ship touches a star.
* **Dynamic Particle Systems:** A custom particle engine that creates golden explosions upon collection, featuring automatic memory cleanup (garbage collection) once particles fade out.
