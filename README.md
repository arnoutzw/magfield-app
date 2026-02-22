# MagField - Magnetic Field Calculator

An interactive 3D magnetic field visualization and calculation tool for exploring electromagnetic fields with various geometries and configurations.

## Screenshots

[Screenshot placeholder - 3D magnetic field visualization with slice planes]

## Features

- **Multiple Geometries** - Calculate fields for:
  - Infinite straight wire
  - Circular coil
  - Solenoid
- **Real-Time Field Magnitude Calculation** - Compute magnetic field strength at any point
- **3D Vector Visualization** - View field vectors in 3D space
- **Field Line Display** - Visualize magnetic field lines for intuitive understanding
- **Customizable Slice Planes** - View cross-sections in XZ, XY, YZ planes or full 3D
- **Field Density Control** - Adjust visualization density for different levels of detail
- **Formula Display** - Shows theoretical formulas with educational context
- **Installable PWA** - Works offline and installs as native-like app

## Tech Stack

- HTML5
- JavaScript
- Three.js
- WebGL
- Progressive Web App (PWA)

## Getting Started

### Quick Start

1. **Online Demo**: Visit [MagField Live](https://arnoutzw.github.io/magfield-app/)
2. **Local Setup**: Clone the repository and open `index.html` in your web browser

```bash
git clone https://github.com/arnoutzw/magfield-app.git
cd magfield-app
# Open index.html in your browser
```

### Installation

This is a PWA that works entirely in your browser with no server or dependencies required. For best experience:
- Install as a PWA on your device for offline access
- Use a modern web browser with WebGL support (Chrome, Firefox, Safari, Edge)

## Usage

1. **Select Geometry**: Choose the source geometry (wire, coil, or solenoid)
2. **Adjust Parameters**: Modify current, radius, dimensions, and other properties
3. **View Field**: Observe the magnetic field visualization in real-time
4. **Change Perspective**: Switch between 3D view and 2D slice planes
5. **Study Theory**: Review formulas and theoretical context


## Theme Support

The app supports two themes:

- **Dark** (default) - Dark background with amber accents
- **ASML Light** - Light theme following ASML corporate design (deep blue #10069f, cyan accents)

When embedded in the Black Sphere Industries portal, theme changes are communicated via `postMessage`:

```javascript
// Sent to parent when theme changes
window.parent.postMessage({ type: "theme-change", theme: "dark" | "asml" }, "*");
```

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Author

Created by arnoutzw
