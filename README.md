# Super Mario 3D 🍄

A 3D Super Mario game built with Three.js for a Computer Graphics course project. Features classic platformer mechanics with modern 3D graphics, multiple levels, coins, and enemies.

![Super Mario 3D](https://img.shields.io/badge/Three.js-v0.160.0-brightgreen) ![Status](https://img.shields.io/badge/Status-Complete-success)

## ✨ Features

- **3D Graphics**: Built using Three.js with real-time rendering and shadows
- **Player Controls**: Smooth WASD/Arrow key movement and spacebar jumping
- **Multiple Levels**: 10 levels with increasing difficulty (levels 6-10 are advanced)
- **Collectibles**: Coins scattered throughout levels to collect
- **Enemies**: Spike Top enemies with collision detection
- **Menu System**: Main menu with level selection and controls display
- **Camera System**: Dynamic third-person camera that follows the player
- **Asset Loading**: Custom asset manager for efficient 3D model loading

## 🎮 Controls

| Key | Action |
|-----|--------|
| **WASD** or **Arrow Keys** | Move Mario |
| **Spacebar** | Jump |
| **Enter** | Start game / Continue to next level |

## 📁 Project Structure

```
super mario/
├── index.html          # Main HTML file
├── main.js             # Game initialization and main loop
├── style.css           # Game styling
├── js/                 # JavaScript modules
│   ├── AssetManager.js # 3D asset loading system
│   ├── Camera.js       # Camera controller
│   ├── Coin.js         # Coin collectible class
│   ├── Enemy.js        # Enemy AI and collision
│   ├── Level.js        # Level generation and management
│   └── Player.js       # Player physics and controls
└── assets/             # 3D models and textures
    ├── lm3_-_mario_mario_thats_his_full_name.glb
    ├── spike_top_super_mario_bros.glb
    └── textures/
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- A local web server (required for loading ES6 modules)

### Installation & Running

1. **Clone or download** this repository

2. **Start a local web server** in the project directory:

   **Using Python:**
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```

   **Using Node.js (http-server):**
   ```bash
   npx http-server -p 8000
   ```

   **Using VS Code:**
   - Install the "Live Server" extension
   - Right-click on `index.html` and select "Open with Live Server"

3. **Open your browser** and navigate to:
   ```
   http://localhost:8000
   ```

4. **Play the game!** Click "Play Game" or press Enter to start

## 🎯 Gameplay

### Objective
Collect all coins in each level while avoiding enemies to progress to the next level.

### Levels
- **Levels 1-5**: Standard difficulty (green buttons in menu)
- **Levels 6-10**: Advanced difficulty (red buttons in menu)

### Tips
- Watch out for Spike Top enemies - they patrol platforms
- Collect all coins to complete each level
- Use the level select menu to jump to specific levels
- Time your jumps carefully to avoid falling off platforms

## 🛠️ Technical Details

### Technologies Used
- **Three.js v0.160.0**: 3D graphics library
- **ES6 Modules**: Modern JavaScript module system
- **GLTF/GLB Models**: 3D assets for player and enemies
- **WebGL**: Hardware-accelerated graphics rendering

### Key Components

#### AssetManager
Handles downloading and caching of 3D models (`.glb` files) asynchronously.

#### Player
- Physics-based movement with gravity and jumping
- Collision detection with platforms
- Model animation and rendering
- Keyboard input handling

#### Level
- Procedural platform generation
- Coin and enemy spawning
- Level progression system
- Scene management

#### Enemy
- Patrol behavior with platform boundaries
- Collision detection with player
- 3D model rendering and animation

#### Camera
- Third-person perspective following the player
- Smooth camera transitions

## 📝 Development Notes

### Browser Compatibility
- Requires a browser with ES6 module support
- WebGL support is required for 3D rendering
- Tested on Chrome, Firefox, and Edge

### Known Issues
- Must be run on a local server (won't work with `file://` protocol)
- Some levels may have performance variations depending on hardware

## 🎓 Academic Context

This project was created for:
- **Course**: 5th Semester Computer Graphics
- **Focus**: Real-time 3D graphics, game physics, and interactive applications
- **Technologies**: Three.js, WebGL, JavaScript ES6

## 📜 License

This is an academic project created for educational purposes.

## 🙏 Acknowledgments

- **Three.js** community for excellent documentation
- 3D models sourced from public repositories
- Inspired by the classic Super Mario games by Nintendo

---

**Enjoy the game! 🎮✨**
