# Emotion Reactive Universe 🌌

An interactive, browser-based generative art project that uses **Computer Vision** to map human emotions into a 3D particle universe. Built with **Three.js** for high-performance graphics and **MediaPipe Face Mesh** for real-time biometric tracking.

## 🚀 Overview

This project creates a "Logic & Color Universe" where 20,000+ particles respond dynamically to your facial expressions. By analyzing landmarks on the user's face, the system identifies emotional states and triggers complex mathematical transformations in 3D space.

### Key Features
* **Real-time Face Tracking:** Uses MediaPipe to track 468+ facial landmarks.
* **EAR (Eye Aspect Ratio) Detection:** Specialized logic to detect blinks, which triggers a "Cosmic Firework" expansion.
* **Dynamic Morphing:** Particles transition smoothly between shapes (Spheres, Spirals, Supernovas) using linear interpolation (LERP).
* **Emotion Mapping:** * **Happy:** Golden Spiral formation with yellow/white hues.
    * **Excited:** High-energy supernova expansion with magenta highlights.
    * **Surprised:** Shockwave expansion in cyan.
    * **Angry:** Compact gravitational core heating up to red/orange.
    * **Neutral:** Stable teal sphere in equilibrium.

## 🛠️ Tech Stack
* **Frontend:** HTML5, CSS3 (HUD overlay)
* **Graphics:** [Three.js](https://threejs.org/) (WebGL)
* **AI/Vision:** [MediaPipe Face Mesh](https://google.github.io/mediapipe/solutions/face_mesh)
* **Mathematics:** Trigonometric functions for shape generation and EAR formulas for blink detection.

## 📂 File Structure
- `emo-particles.html`: The initial version featuring core emotion heuristics and basic particle shapes.
- `emo2-particle.html`: Version 1.2 (Logic & Color Patch) with EAR blink detection, improved color transitions, and 20,000 particle support.

## 🚦 Getting Started
1. Clone the repository.
2. Open either `.html` file in a modern web browser (Chrome or Edge recommended).
3. Grant camera permissions when prompted.
4. Experiment with facial expressions and watch the universe react!

## 🧪 Math Behind the Magic

The project utilizes the **Eye Aspect Ratio (EAR)** to detect blinks:

$$EAR = \frac{||p_2 - p_6|| + ||p_3 - p_5||}{2||p_1 - p_4||}$$

This ensures that the "Firework" effect is triggered by physical blinks rather than general movement.
