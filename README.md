# 🔥 WebGL Fluid Simulation

An insanely high-performance, purely customized WebGL fluid simulation running natively in your browser using the **Navier-Stokes equations**. The system accurately models fluid advection, divergence, curl, and pressure solving within an intricately optimized Fragment Shader pipeline.

[👉 Live Demo](https://fluid-simulation-sand.vercel.app/)

## 🚀 Key Features

*   **V1 & V2 Dual Architecture:**
    *   **V1 (Core Engine):** A hyper-stable, ultra-responsive Naviar-Stokes sandbox.
    *   **V2 (Advanced Physics):** An experimental zone featuring:
        *   **Image Dissolve:** Dynamically inject textures to melt into the dye sequence via a restorative force.
        *   **Thermal Convection:** "Lava-lamp" physics driving buoyancy offsets based on an isolated Temperature ping-pong buffer.
        *   **Static SDF Boundaries:** A procedural Signed Distance Field forcing no-slip fluid flow around central obstacles.
*   **Custom Glassmorphic UI:** Removed all external dependencies (no dat.gui). Fully responsive, mobile-compliant glassmorphism UI overlay.
*   **URL State Management:** Every parameter is continuously serialized down to the `window.location.hash` allowing flawless instant sharing presets!
*   **Post-Processing Pipeline:** Multi-pass Bloom prefilters, Sunray light scattering, blurring, and dithering natively baked in.

## 🛠️ Quick Start (Local Development)

The codebase has exactly zero `npm` dependencies. To run it flawlessly:

1.  Clone the repository:
    ```bash
    git clone https://github.com/captain-america-7/Fluid-Simulation.git
    cd Fluid-Simulation
    ```
2.  Launch a simple static file server (e.g. using Python or Node):
    ```bash
    npx serve .
    # OR
    python -m http.server 8000
    ```
3.  Visit `http://localhost:3000` (or `8000`) in your browser.

## 🤝 Building & Contributing

Feel free to break it and evolve it. 

1. **Fork the repo** and create a feature branch (`git checkout -b feature-amazing-fluid`).
2. **Review `script.js` or `v2.js`**: WebGL initialization limits are explicitly handled inside `initFramebuffers()`.
3. **Commit** your fluid mechanic (e.g., `git commit -m 'feat: Add non-Newtonian viscosity shader'`).
4. **Push & Pull Rquest**.

## 🎨 License

This project is open-source. Fork it, rip the shaders, build beautiful things.
 element + floating UI chrome.
- `script.js`: Physics engine + WebGL core. Follows a functional setup and uses heavily optimised GLSL kernels.
- Pure HTML/CSS UI: Control inputs styled to match the custom glassmorphic aesthetic (no external UI libraries required).
- `LDR_LLL1_0.png`: Dithering noise texture to eliminate color banding.

## Features
- Multi-touch fluid splats with responsive color transitions.
- Automatic performance scaling (degrades cleanly on low-end hardware).
- Zero-friction URL State persistence for sharing presets (e.g. `/#viscosity=0.4&bloom=true`).
- Accessible, single-page architecture built purely with ES6 and WebGL.

## Contributing

See ["Good first issues"](https://github.com/paveldogreat/WebGL-Fluid-Simulation/issues) for an entry point. Read `CONTRIBUTING.md` for specific contribution workflows and rules.
