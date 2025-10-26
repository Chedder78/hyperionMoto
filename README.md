# VELOCITY MOTO - Custom Supersport Motorcycles

![Velocity Moto](https://img.shields.io/badge/Velocity-Moto-ff2a00?style=for-the-badge&logo=motorcycle&logoColor=white)
![Version](https://img.shields.io/badge/version-1.0.0-1a1a1a?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-00e5ff?style=for-the-badge)

A premium website for Velocity Moto, showcasing custom supersport motorcycles with an immersive AR/VR showroom experience.

## 🚀 Features

### Core Website
- **Responsive Design** - Optimized for all devices
- **Multi-page Navigation** - Smooth transitions between sections
- **Motorcycle Models** - Detailed showcase of Vulcan S1, Apex R9, and Nitro ZX
- **Customization Tool** - Interactive bike customization interface
- **Build Process** - Step-by-step customization workflow
- **Contact Integration** - Customer inquiry forms

### AR/VR Showroom
- **3D Motorcycle Visualization** - Interactive 3D models in virtual space
- **Multiple Experience Modes** - Desktop, VR, and AR compatibility
- **WebXR Integration** - Built with Three.js for cross-platform compatibility
- **Immersive Controls** - Mouse, keyboard, and VR controller support
- **Real-time Customization** - Visual changes to motorcycle models

## 🛠️ Technology Stack

### Frontend
- **HTML5** - Semantic markup structure
- **CSS3** - Custom properties, Grid, Flexbox, animations
- **JavaScript ES6+** - Modern JavaScript features
- **Three.js** - 3D graphics and WebGL rendering
- **WebXR API** - Virtual and augmented reality

### Libraries & Dependencies
- **Three.js r128** - 3D graphics library
- **OrbitControls** - Camera controls for 3D scenes
- **GLTFLoader** - 3D model loading
- **Font Awesome 6.4.0** - Icons
- **Google Fonts** - Orbitron & Exo 2 typography

## 📁 Project Structure

```
velocity-moto/
├── index.html                 # Main website file
├── README.md                  # Project documentation
├── assets/
│   ├── images/               # Static images and textures
│   ├── models/               # 3D model files (.glb, .gltf)
│   └── audio/                # Sound effects and audio
├── css/
│   ├── style.css             # Main stylesheet
│   ├── ar-vr.css            # AR/VR specific styles
│   └── responsive.css        # Media queries
└── js/
    ├── main.js               # Core website functionality
    ├── ar-vr-engine.js      # AR/VR scene management
    ├── models.js            # 3D model handling
    ├── ui-manager.js        # User interface controls
    └── utils.js             # Utility functions
```

## 🎯 Pages & Sections

### Main Pages
1. **Home** - Hero section, features, model showcase
2. **Models** - Detailed motorcycle specifications
3. **Customization** - Interactive bike builder
4. **AR/VR Showroom** - Immersive 3D experience
5. **Gallery** - Portfolio of custom builds
6. **About** - Company story and team
7. **Contact** - Customer inquiry forms

### AR/VR Features
- **Desktop Mode** - Mouse and keyboard controls
- **VR Mode** - Virtual reality headset support
- **AR Mode** - Augmented reality on mobile devices
- **Interactive Models** - Click to view specifications
- **Real-time Rendering** - 60fps 3D graphics

## 🚀 Quick Start

### Prerequisites
- Modern web browser with WebGL support
- For VR: WebXR-compatible headset (Oculus, HTC Vive, etc.)
- For AR: ARCore (Android) or ARKit (iOS) compatible device

### Installation
1. Clone the repository:
```bash
git clone https://github.com/your-username/velocity-moto.git
cd velocity-moto
```

2. Serve the files using a local server:
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

3. Open your browser and navigate to:
```
http://localhost:8000
```

## 🎮 Usage

### Website Navigation
- Use the navigation menu to switch between pages
- Click "Build Yours" to start customization
- Explore motorcycle models with detailed specifications

### AR/VR Controls
**Desktop Mode:**
- `Mouse` - Look around
- `WASD` - Move around the showroom
- `Click` - Select motorcycles
- `Space` - Cycle through models

**VR Mode:**
- Connect VR headset and click "ENTER VR"
- Use motion controllers for interaction
- Teleport or smooth locomotion

**AR Mode:**
- Mobile device with AR support required
- Move device to explore virtual objects in real space
- Tap to place and interact with models

## 🎨 Customization

### Design System
- **Primary Color**: `#ff2a00` (Velocity Red)
- **Secondary**: `#1a1a1a` (Dark Gray)
- **Accent**: `#00e5ff` (Electric Blue)
- **Text**: `#f5f5f5` (Light Gray)
- **Background**: `#0a0a0a` (Near Black)

### Adding New Motorcycle Models
1. Add model data to `motorcycleData` array:
```javascript
{
    name: "Model Name",
    description: "Model description",
    power: "300 HP",
    weight: "140 kg", 
    speed: "350 km/h",
    color: 0x2a2a2a
}
```

2. Add 3D model files to `assets/models/`
3. Update the customization options as needed

## 🔧 Development

### Building for Production
```bash
# Minify CSS
npx css-minify -f style.css -o dist/

# Minify JavaScript  
npx uglify-js js/main.js -o dist/main.min.js

# Optimize images
npx imagemin assets/images/* --out-dir=dist/images
```

### Browser Support
- Chrome 90+ (Recommended)
- Firefox 88+
- Safari 14+
- Edge 90+

### Performance Optimization
- Lazy loading for 3D models
- Compressed textures (WebP format)
- GLTF/GLB model optimization
- Code splitting for large JavaScript files

## 🌐 Deployment

### Static Hosting (Recommended)
- **Netlify**: Drag and drop the `index.html` file
- **Vercel**: Connect GitHub repository for automatic deployments
- **GitHub Pages**: Push to `gh-pages` branch

### Server Requirements
- Static file serving
- HTTPS enabled (required for WebXR)
- MIME types for GLTF/GLB files:
```
model/gltf+json .gltf
model/gltf-binary .glb
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Setup
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

### Code Style
- Use semantic HTML5 elements
- Follow CSS BEM methodology
- ES6+ JavaScript with consistent formatting
- Comment complex 3D rendering code

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🐛 Known Issues

- [ ] Mobile AR requires additional permission handling
- [ ] VR controller mapping needs device-specific testing
- [ ] Large 3D models may impact performance on low-end devices
- [ ] Safari WebXR support limited to iOS 13+

## 🚧 Roadmap

### Phase 1 (Current)
- [x] Basic website structure
- [x] AR/VR integration
- [x] Motorcycle customization
- [x] Responsive design

### Phase 2 (Next)
- [ ] Real 3D model integration
- [ ] Advanced customization options
- [ ] E-commerce integration
- [ ] User accounts

### Phase 3 (Future)
- [ ] Multiplayer VR showroom
- [ ] Advanced physics simulations
- [ ] Mobile app development
- [ ] Internationalization

## 📞 Support

For support and questions:
- 📧 Email: dev@velocitymoto.com
- 🐛 [Issue Tracker](https://github.com/your-username/velocity-moto/issues)
- 💬 [Discord Community](https://discord.gg/velocitymoto)

## 🙏 Acknowledgments

- Three.js community for excellent 3D web graphics
- WebXR Device API for immersive experiences
- Unsplash for high-quality motorcycle imagery
- Font Awesome for beautiful icons

---

<div align="center">

**Built with passion for motorcycle enthusiasts everywhere** 🏍️

*Experience the future of motorcycle customization today*

</div>
