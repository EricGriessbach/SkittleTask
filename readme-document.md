# Ball Trajectory Game

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

An interactive physics-based simulation of a ball trajectory task inspired by research on motor learning and skill acquisition.

![Ball Trajectory Game Preview](preview.png)

## 📖 Description

This web-based simulation implements a classic motor learning task where users must launch a ball around a central pole to hit a target on the opposite side. The physics model creates realistic elliptical trajectories based on a damped oscillator system.

This simulation is based on the experimental paradigm described in:
> Müller, H., & Sternad, D. (2004). Decomposition of Variability in the Execution of Goal-Oriented Tasks: Three Components of Skill Improvement. Journal of experimental psychology. Human perception and performance, 30(1), 212-33. https://doi.org/10.1037/0096-1523.30.1.212

## ✨ Features

- **Realistic Physics**: Implementation of damped oscillatory motion with spring-mass dynamics
- **Interactive Controls**: Adjust launch velocity and angle in real-time
- **Visual Feedback**: See the complete trajectory and the point of minimum distance to target
- **Performance Metrics**: Measure the minimum distance to target and when it occurs
- **Parameter Heat Map**: Visualize how different velocity/angle combinations affect performance
- **Responsive Design**: Works across different screen sizes

## 🚀 Demo

Try the live demo: [Ball Trajectory Game](https://your-username.github.io/ball-trajectory-game)

## 🛠️ Installation

### Option 1: Direct Download
1. Download or clone this repository
   ```bash
   git clone https://github.com/your-username/ball-trajectory-game.git
   ```
2. Open `index.html` in your web browser

### Option 2: Using as a Component
Include the HTML file in your existing project and customize as needed.

## 💻 Usage

1. Adjust the velocity magnitude slider (0.5 to 3.0)
2. Set the launch angle (0° to 359°)
3. Click "Launch Ball" to run the simulation
4. Observe the ball's trajectory and its minimum distance to the target
5. Use the parameter map to identify optimal launch settings

## 🧮 Physics Model

The ball follows a trajectory defined by the equations:

```
x(t) = A_x sin(ωt + φ_x)e^(-t/τ)
y(t) = A_y sin(ωt + φ_y)e^(-t/τ)
```

Where:
- Initial position: (0, -1.5)
- Target position: (0.35, 1)
- Mass: 0.1 kg
- Spring constant: 1 N/m
- Damping factor (τ): 20
- Angular frequency (ω): 3.16 rad/s

## 🔬 Research Applications

This simulation can be used to study:

- **Motor Learning**: How users improve with practice
- **Skill Acquisition**: Analysis of variability components (tolerance, noise, covariation)
- **Human-Computer Interaction**: Understanding parameter exploration strategies

## 🧩 Project Structure

```
ball-trajectory-game/
├── index.html         # Main simulation file with HTML, CSS, and JavaScript
├── README.md          # This documentation
└── preview.png        # Screenshot of the application
```

## 🔧 Customization

You can modify various aspects of the simulation:

- **Physics Parameters**: Edit the constants at the top of the script
- **Visual Styling**: Adjust the CSS variables for colors and dimensions
- **Difficulty**: Change the target position or central post size

## 📱 Browser Compatibility

Tested and working on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- Müller, H., & Sternad, D. for the original research and task design
- The HTML5 Canvas API for rendering capabilities
