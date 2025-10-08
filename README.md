# 🪔 AR Rangoli Viewer - Diwali Special

An interactive web-based Augmented Reality (AR) application that lets you place beautiful virtual rangoli patterns in your real environment using your device's camera. Perfect for celebrating Diwali with a modern twist!

## ✨ Features

- **Real-time AR Experience**: View virtual rangoli patterns overlaid on your real environment
- **Multiple Rangoli Patterns**: Choose from 5 different traditional designs:
  - Floral Rangoli
  - Geometric Rangoli
  - Peacock Rangoli
  - Mandala Rangoli
  - Diya Rangoli
- **Interactive Placement**: Place multiple rangoli patterns anywhere in your camera view
- **Animated Effects**: All rangoli patterns feature smooth rotation and floating animations
- **Screenshot Capability**: Capture and save your AR creations
- **Mobile Responsive**: Works on smartphones and tablets with camera access
- **No App Installation Required**: Runs directly in web browsers

## 🚀 Live Demo

Visit: [https://jainks1996.github.io/ar-rangoli-viewer/](https://jainks1996.github.io/ar-rangoli-viewer/)

## 📱 System Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Device with camera (smartphone, tablet, or computer with webcam)
- Internet connection (for loading AR libraries)

## 🛠️ Technologies Used

- **A-Frame**: Web framework for building VR/AR experiences
- **AR.js**: Augmented Reality for the web
- **HTML5/CSS3**: Frontend structure and styling
- **JavaScript**: Interactive functionality
- **WebRTC**: Camera access and streaming

## 💻 Local Development

1. Clone the repository:
```bash
git clone https://github.com/jainks1996/ar-rangoli-viewer.git
cd ar-rangoli-viewer
```

2. Start a local server (required for camera access):
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server

# Using VS Code Live Server extension
# Right-click on index.html and select "Open with Live Server"
```

3. Open in browser:
```
http://localhost:8000
```

## 📦 Deployment on GitHub Pages

1. Push your code to GitHub:
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. Enable GitHub Pages:
   - Go to repository Settings
   - Navigate to Pages section
   - Select Source: Deploy from a branch
   - Select Branch: main
   - Select Folder: / (root)
   - Click Save

3. Your site will be available at:
```
https://yourusername.github.io/ar-rangoli-viewer/
```

## 🎮 How to Use

1. **Grant Camera Permission**: Allow the website to access your camera when prompted
2. **Point at Floor**: Aim your camera at a flat surface (floor works best)
3. **Select Pattern**: Choose your favorite rangoli design from the dropdown
4. **Place Rangoli**: Click "Place Rangoli" to add it to your view
5. **Add More**: Place multiple rangoli patterns to create elaborate decorations
6. **Capture**: Use the capture button to save screenshots of your creation

## 🎨 Customization

### Adding New Rangoli Patterns

Edit the `script.js` file and add new pattern functions:

```javascript
function createCustomRangoli(parent) {
    // Add your custom rangoli design here
    const element = document.createElement('a-entity');
    // Configure your pattern
    parent.appendChild(element);
}
```

### Modifying Colors

Change the color schemes in the pattern creation functions:

```javascript
const colors = ['#ff6b6b', '#ffd93d', '#ff9ff3']; // Your custom colors
```

### Adjusting Animations

Modify animation parameters in the `createRangoliPattern` function:

```javascript
rangoli.setAttribute('animation__rotate', {
    property: 'rotation',
    to: '0 360 0',
    loop: true,
    dur: 30000, // Change rotation speed
    easing: 'linear'
});
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/NewRangoli`)
3. Commit your changes (`git commit -m 'Add new rangoli pattern'`)
4. Push to the branch (`git push origin feature/NewRangoli`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- A-Frame team for the amazing AR/VR framework
- AR.js contributors for bringing AR to the web
- Traditional rangoli artists for design inspiration

## 🐛 Known Issues

- Camera access must be granted for AR to work
- Works best in well-lit environments
- Some older devices may experience performance issues with multiple rangoli patterns

## 📞 Support

For issues or questions, please create an issue in the GitHub repository or contact [your-email@example.com]

## 🎉 Happy Diwali!

May your celebrations be filled with light, joy, and beautiful rangoli patterns - both real and virtual!

---

Made with ❤️ for Diwali