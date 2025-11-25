# ⚽ AR Soccer

An immersive Augmented Reality soccer game built with WebXR and Three.js. Place a virtual soccer ball in your real environment and kick it using your Android device!

![AR Soccer](https://img.shields.io/badge/WebXR-AR-blue) ![Three.js](https://img.shields.io/badge/Three.js-r128-green) ![License](https://img.shields.io/badge/license-MIT-orange)

## 🎮 Features

- **Immersive AR Experience**: Place and interact with a 3D soccer ball in your real environment
- **Realistic Physics**: Ball physics with gravity, bouncing, and friction
- **Multiplayer Ready**: Room-based system for hosting and joining games
- **Mobile Optimized**: Built specifically for Android devices with ARCore support

## 📱 Requirements

- **Android Device** with ARCore support
- **Chrome Browser** (latest version)
- **ARCore** installed from Google Play Store

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)
Visit the live demo: `https://z1000biker.github.io/ar-soccer`

### Option 2: Local Development

1. Clone the repository:
```bash
git clone https://github.com/z1000biker/ar-soccer.git
cd ar-soccer
```

2. Start a local server:
```bash
# Using Python 3
python -m http.server 8080

# Or using Node.js
npx http-server -p 8080
```

3. Access from your Android device:
   - Connect to the same network as your computer
   - Open Chrome and navigate to `http://YOUR_COMPUTER_IP:8080`

## 🎯 How to Play

1. **Setup**: Enter your name and either host a new game or join an existing room
2. **Start AR**: Tap "Start AR" and grant camera permissions
3. **Place Ball**: Point your device at a flat surface and tap to place the ball
4. **Kick**: Tap again to kick the ball in the direction you're facing
5. **Have Fun**: Watch the ball bounce and roll with realistic physics!

## 🛠️ Technology Stack

- **WebXR Device API**: For AR session management
- **Three.js (r128)**: 3D graphics rendering
- **ARCore**: Android's AR platform
- **Vanilla JavaScript**: No framework dependencies

## 📂 Project Structure

```
ar-soccer/
├── index.html          # Main application file
├── README.md          # This file
└── LICENSE            # MIT License
```

## 🔧 Technical Details

### AR Features
- Hit-test API for surface detection
- Real-time tracking with 6DOF
- Local floor reference space
- Reticle for placement guidance

### Physics Simulation
- Gravity: 9.8 m/s²
- Bounce coefficient: 0.7
- Ground friction: 0.95
- Air resistance: 0.98

### 3D Rendering
- Hemisphere lighting for realistic shadows
- Standard PBR materials
- Smooth ball rotation based on velocity

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Three.js](https://threejs.org/)
- Powered by [WebXR](https://immersiveweb.dev/)
- AR by [ARCore](https://developers.google.com/ar)

## 📞 Contact

Created by [@z1000biker](https://github.com/z1000biker)

---

**Note**: This is the current stable version. A leg-tracking version using TensorFlow.js MoveNet is in development for more immersive kick detection!
