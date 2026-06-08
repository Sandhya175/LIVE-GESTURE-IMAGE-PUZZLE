# 🧩 Live Gesture Image Puzzle

> **Turn Your World into a Game.** Forget the mouse and keyboard—your hands are the controllers.

"Live Gesture Image Puzzle" is an interactive, browser-based game that transforms your real-time webcam feed into a playable, physical puzzle using advanced AI hand-tracking.

---

## 🎮 How it Works

The experience is broken down into intuitive, gesture-based phases:

### 📸 Phase 1: Capture (The Setup)
* **Frame the Shot:** Look at your webcam feed and use both hands to create an "L" shape (like a movie director framing a scene). The AI detects this gesture and draws a bounding box on the screen.
* **Snap the Picture:** While holding the frame, pinch the index finger and thumb of both hands together simultaneously. This acts as the camera shutter, taking a snapshot of whatever is inside your hand frame.
* **The Transformation:** The game instantly takes that captured area, crops it, and shuffles it into a 3x3 sliding tile puzzle right before your eyes.

### 🧩 Phase 2: Solve (The Game)
* **Pinch to Pick Up:** Hover your hand over a puzzle tile. The cursor will follow your hand. Pinch your index finger and thumb together to "grab" the tile.
* **Drag & Drop to Swap:** While holding the pinch, move your hand to drag the tile to a new location on the grid. Release the pinch to drop it and swap positions with the tile underneath.
* **Race the Clock:** A timer starts as soon as the puzzle is generated. Use your hand-eye coordination to solve the image as quickly as possible.
* **Need a Reset?:** Made a mistake or want a new image? Simply close one hand into a fist and hold it for 1.5 seconds. The game will reset back to the capture phase.

### 🏆 Phase 3: The Leaderboard (The Glory)
* **Victory:** Once you successfully arrange all the tiles back into their original picture, the game is solved!
* **Log Your Time:** You'll be prompted to enter your name (using your keyboard) to log your time.
* **Compete Globally:** Your score is instantly uploaded to a live, real-time leaderboard where you can compare your speed against other players worldwide. The leaderboard also tracks your personal best times.

---

## 🛠️ Under the Hood

Live Gesture Image Puzzle is a unique blend of computer vision, quick-thinking puzzle mechanics, and competitive social features, offering a fast-paced and highly interactive web experience.

* **🤖 AI Hand Tracking:** Powered by `@mediapipe/tasks-vision`, the game uses a lightweight, highly responsive machine learning model right in your browser to track hand landmarks (joints and fingertips) in real-time.
* **☁️ Real-time Multiplayer Backend:** The leaderboard is powered by **Firebase Firestore**, ensuring that as soon as someone sets a new high score, it updates instantly for everyone currently playing.
* **✨ Smooth UI:** Built with **React** and **HTML5 Canvas**, the visuals feature sleek animations, glowing custom cursors, and intuitive overlays that guide you through the process without needing lengthy tutorials.
