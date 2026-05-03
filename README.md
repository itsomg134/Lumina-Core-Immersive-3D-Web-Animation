#  Lumina Core – Immersive 3D Web Animation

![Preview](https://via.placeholder.com/800x400?text=Lumina+Core+Animation)  
*A dynamic, interactive 3D particle universe built with Three.js.*

Lumina Core is a visually stunning web animation experience featuring a glowing torus knot at its heart, surrounded by thousands of colorful particles, dynamic lighting, and subtle mouse-driven parallax. It’s designed to showcase the creative potential of real-time 3D graphics in the browser.

[![Live Demo](https://img.shields.io/badge/Live_Demo-View_Here-6C3BFF?style=for-the-badge&logo=vercel)](https://your-demo-link.com)  
[![Three.js](https://img.shields.io/badge/Three.js-r128-000000?style=for-the-badge&logo=threedotjs)](https://threejs.org/)

---

##  Features

- **Central Animated Geometry** – A metallic torus knot with a glowing inner sphere, rotating in 3D space.
- **Massive Particle Systems** – Over 14,000 colored particles forming a nebula-like cloud, plus distant stars and floating dust.
- **Dynamic Lighting** – Moving point lights, color‑shifting rim lights, and a pulsating core glow.
- **Interactive Effects** – Mouse movement creates subtle camera parallax. Click the **“Explore Nebula”** button to trigger a light burst and particle flash.
- **Orbital & Wavy Rings** – Rotating particle rings and semi‑transparent wireframe loops add depth.
- **Fully Responsive** – Adapts to any screen size with high‑DPI support.

---

##  Controls & Interaction

| Action                     | Effect                                 |
| -------------------------- | -------------------------------------- |
| **Move mouse**             | Smooth camera parallax (look around)   |
| **Click “Explore Nebula”** | Temporary light burst + particle pulse |
| **No further input needed**| Scene animates automatically           |

---

##  Technology Stack

- [Three.js](https://threejs.org/) (r128) – Core 3D library
- HTML5 / CSS3 – Overlay styling & responsive layout
- JavaScript (ES6) – Animation logic & interactivity
- WebGL – Hardware‑accelerated rendering

---

##  Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/lumina-core.git
cd lumina-core
```

### 2. Run locally

Because the project uses ES modules and imports Three.js from a CDN, you can simply serve it with any static server. For example:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (live-server)
npx live-server
```

Then open `http://localhost:8000` in your browser.

> No build step or installation required – just pure HTML/CSS/JS.

---

##  Project Structure

```
lumina-core/
├── index.html          # Main entry point (canvas + UI overlay)
└── README.md           # This file
```

All code (styles, markup, and Three.js logic) is contained in a single `index.html` file for simplicity and ease of deployment.

---

##  Customization

Want to tweak the visuals? Look for these sections in the code:

| Parameter                     | Location in `index.html`                          |
| ----------------------------- | -------------------------------------------------- |
| Particle count & colors       | `PARTICLE_COUNT`, `colorArray` generation         |
| Central knot size / color     | `TorusKnotGeometry`, `knotMaterial`               |
| Light intensities & movement  | `movingLight`, `coreGlow`, `rimLight`             |
| Camera distance / FOV         | `new THREE.PerspectiveCamera(...)`                |
| Animation speeds              | `time` multiplier in `animate()`                  |
| Burst effect strength         | `burstIntensity` handling in click event          |

---

## 🧠 How It Works

1. **Scene Setup** – A dark blue foggy backdrop with multiple light sources.
2. **Core Object** – A torus knot and inner sphere rotate at different rates.
3. **Particle Clouds** – Thousands of vertices with per‑vertex colors create a nebula effect.
4. **Orbital Elements** – Points and line loops rotate around the center.
5. **Animation Loop** – Updates rotations, light positions, camera target, and handles the burst effect.
6. **Mouse Interaction** – Listens to `mousemove` to gently shift camera angles.

---

## 🌍 Browser Support

Works on all modern browsers that support WebGL:

- Chrome / Edge (latest)
- Firefox (latest)
- Safari 15+
- Mobile browsers (iOS Safari, Chrome for Android)

---

## 🤝 Contributing

Contributions, ideas, and improvements are welcome!  
Feel free to open an issue or submit a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-effect`)
3. Commit your changes (`git commit -m 'Add some amazing effect'`)
4. Push to the branch (`git push origin feature/amazing-effect`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙏 Acknowledgments

- Built with [Three.js](https://threejs.org/) – the amazing 3D library for the web.
- Inspiration from cosmic art and generative particle aesthetics.
- Fonts from Google Fonts (Poppins) via system fallback.

---

## 📬 Contact

Your Name – [@yourhandle](https://twitter.com/yourhandle) – email@example.com

Project Link: [https://github.com/your-username/lumina-core](https://github.com/your-username/lumina-core)

---

*Made with ✨ and JavaScript*
```
