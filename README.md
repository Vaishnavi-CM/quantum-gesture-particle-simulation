# ⚛️ Quantum Gesture Particle Simulation

### Interact with a dynamic particle universe using hand gestures.

A browser-based interactive graphics project that combines computer vision, gesture recognition, and particle animation. Using a webcam, users can control the behavior of a glowing particle system through natural hand movements.

Built with **HTML5, CSS3, JavaScript, Canvas API, and MediaPipe Hands**.

## ✨ Features

- **Real-Time Hand Tracking** — Detects hand landmarks using MediaPipe Hands.
- **Gesture-Based Controls** — Maps recognized hand gestures to particle effects.
- **Interactive Particle System** — Simulates repulsion, attraction, swirling motion, and velocity damping.
- **Dynamic Visual Effects** — Includes glowing particles, connecting lines, motion trails, and changing colors.
- **Live FPS Counter** — Displays a frame-rate measurement to help observe animation performance.
- **Futuristic User Interface** — Features a dark theme, glass-inspired panels, neon accents, and an on-screen gesture guide.
- **Responsive Canvas** — Resizes the animation canvas to match the browser window.

## 🖐️ Gesture Controls

| Hand gesture | Particle behavior | Color theme |
|---|---|---|
| 🖐️ Open palm | Repels nearby particles | Cyan |
| ✊ Closed fist | Attracts particles toward the hand | Magenta / Red |
| 🤏 Thumb and index finger pinch | Creates a swirling motion | Orange |
| ✌️ Peace sign | Strongly slows particle movement | Lavender |

> Gesture recognition is based on hand-landmark geometry. Results may vary with lighting, hand orientation, webcam quality, and tracking conditions. The peace-sign mode applies strong velocity damping rather than a mathematically complete freeze.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure and webcam video element |
| CSS3 | Layout, styling, and visual effects |
| JavaScript (ES6+) | Gesture classification, particle logic, and animation |
| Canvas API | Real-time rendering of particles and connecting lines |
| MediaPipe Hands | Hand landmark detection |
| MediaPipe Camera Utils | Webcam frame capture and processing |
| jsDelivr CDN | Delivery of external MediaPipe libraries |

## ⚙️ How It Works

1. **Camera input:** The browser captures webcam frames after the user grants permission.
2. **Hand tracking:** MediaPipe Hands estimates hand landmarks from the frames.
3. **Gesture classification:** JavaScript compares landmark distances to identify supported gestures.
4. **Particle simulation:** The detected gesture influences particle forces, velocity, and color.
5. **Rendering:** The Canvas API continuously draws the particle field and its visual effects.

The application does not require a dedicated backend server. It relies on browser APIs and externally loaded MediaPipe libraries.

## 🚀 Getting Started

### Requirements

- A modern web browser, preferably Google Chrome.
- A working webcam.
- Internet access to load the MediaPipe dependencies and models.
- Camera permission enabled for the page.

### Run Locally

1. Download this repository or clone it to your computer.
2. Open the project folder in Visual Studio Code or another editor.
3. Serve `quantum_v3.html` using a local development server, such as the Live Server extension in Visual Studio Code.
4. Open the local URL shown by the server.
5. Allow camera access when prompted.
6. Follow the on-screen gesture guide to interact with the particle simulation.

**Important:** Webcam access generally requires a secure context, such as `localhost` or an HTTPS website. Opening the HTML file directly may not work consistently across browsers.

## 📂 Project Structure

```text
quantum-gesture-particle-simulation/
├── quantum_v3.html   # Main application
└── README.md         # Project documentation
```

The main HTML file contains the page structure, CSS styling, JavaScript logic, particle simulation, and MediaPipe integration.

## 🎓 What This Project Demonstrates

- Integrating a browser-based computer vision library.
- Working with hand landmarks and geometric gesture detection.
- Building interactive particle systems.
- Applying forces, velocity damping, and continuous animation.
- Rendering real-time graphics with the Canvas API.
- Handling webcam input and browser camera permissions.
- Combining visual design with interactive functionality.

## 🔮 Future Enhancements

- Add robust camera initialization and permission-error handling.
- Improve gesture recognition stability and reduce accidental mode changes.
- Implement a true pause and resume control for particle motion.
- Add controls for particle count, sensitivity, and simulation settings.
- Optimize rendering for lower-powered devices.
- Add a live demo link and a short demonstration GIF or video.

## 🔐 Privacy

The application uses the webcam to recognize hand gestures. The application code does not implement a custom backend for uploading recorded video. MediaPipe dependencies are loaded externally, so their delivery and runtime behavior depend on those third-party libraries.

Camera access is requested by the browser and requires user permission.

## 📌 Project Status

**Functional prototype — tested locally by the developer.**

The experience may vary depending on the browser, camera, lighting, internet connection, and device performance.

## 👩‍💻 Author

Developed as a hands-on exploration of computer vision, interactive graphics, and gesture-controlled browser experiences.

