# Particle vs String Motion in Spacetime

An interactive 3D visualization demonstrating the fundamental difference between how particles and strings move through spacetime, based on concepts from string theory and general relativity.

## Overview

This project visualizes two key concepts in theoretical physics:

- **Particles** as point objects that trace 1D worldlines through spacetime
- **Strings** as extended objects that sweep out 2D worldsheets as they evolve

The visualization shows how these different types of objects create distinct geometric structures in spacetime, illustrating the principle of least action for both cases.

## Features

- Interactive 3D visualization using Three.js
- Real-time animation of particle and string motion
- Dynamic worldline generation for particles
- Dynamic worldsheet construction for strings
- Mouse controls for rotating and zooming the view
- Toggle between particle view, string view, or both simultaneously

## Physics Concepts Demonstrated

### Particle Motion
- A particle is treated as a point with no spatial extent
- As it moves through spacetime, it traces a one-dimensional curve called a worldline
- The particle follows the path that minimizes proper time (geodesic motion)

### String Motion
- A string is a one-dimensional extended object with length
- Each point on the string traces its own worldline through spacetime
- These worldlines collectively form a two-dimensional surface called a worldsheet
- The string evolves to minimize the area of this worldsheet

### Action Principles
- Point particles minimize the length of their worldline
- Strings minimize the area of their worldsheet
- Both represent applications of the principle of least action in different dimensions

## Technical Implementation

### Core Technologies
- HTML5 Canvas with WebGL rendering
- Three.js for 3D graphics and scene management
- Parametric geometry generation for worldsheet construction
- Real-time geometric calculations for smooth animation

### Key Components

#### Particle System
- Point particle represented as a small sphere
- Worldline generated from historical positions
- Smooth parametric motion using trigonometric functions

#### String System
- String represented as a connected series of points
- Vibration and oscillation effects
- Worldsheet constructed from string's temporal evolution

#### Worldsheet Generation
- Parametric surface construction using historical string positions
- Real-time mesh generation and updating
- Wireframe and solid rendering modes for clarity

## Controls

- **Mouse Drag**: Rotate the camera around the scene
- **Mouse Wheel**: Zoom in and out
- **Show Particle Worldline**: Display only the particle and its worldline
- **Show String Worldsheet**: Display only the string and its worldsheet
- **Show Both**: Display both systems simultaneously
- **Toggle Animation**: Pause or resume the animation
- **Reset View**: Return camera to default position

## Installation and Usage

1. Clone this repository
2. Open `index.html` in a modern web browser
3. Use the control panel to switch between visualization modes
4. Interact with the scene using mouse controls

No additional dependencies or build process required - runs entirely in the browser.

## Educational Applications

This visualization is designed for:
- Physics students learning about spacetime geometry
- Understanding the mathematical foundations of string theory
- Visualizing abstract concepts in theoretical physics
- Demonstrating the principle of least action
- Comparing point particle and field theory approaches

## Mathematical Background

### Worldline Parameterization
The particle worldline is parameterized as:
```
x(t) = A * sin(ωt)
y(t) = B * sin(ω't) 
z(t) = C * cos(ω''t)
```

### Worldsheet Construction
The string worldsheet is generated by evolving the string configuration over time, creating a mapping from (τ, σ) parameter space to spacetime coordinates, where τ represents time evolution and σ represents position along the string.

## Browser Compatibility

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

Requires WebGL support for 3D rendering.

## License

MIT License - feel free to use and modify for educational purposes.

## Contributing

Contributions welcome! Areas for improvement:
- Additional visualization modes
- Enhanced physics accuracy
- Performance optimizations
- Educational annotations
- Mobile device support