# 🚴 GPX Track Replanner

Created and deployed using claude 4.1 fully on mobile during vacation ;)

A web-based tool to replan GPX cycling tracks to start from your location and create perfect loops. Transform any GPX route into a customized loop that begins and ends at your chosen starting point.

![GPX Track Replanner Screenshot](https://aekschen.github.io/gpx-track-replanner/Screenshot.jpg)**)

## ✨ Features

- **📁 Load GPX Files** - Import any GPX track file
- **📍 Multiple Start Options** - Use your current location or pick a point on the map
- **🔄 Loop Creation** - Automatically creates routes that return to your starting point
- **🗺️ Beautiful Maps** - Topographic maps with mountain shading and terrain details
- **⚡ Smart Routing** - Uses OpenRouteService for optimal cycling routes
- **💾 Export GPX** - Download your replanned route as a GPX file
- **🌙 Dark Theme** - Modern dark interface with gradient styling
- **📱 Mobile Friendly** - Responsive design works on all devices

## 🚀 Live Demo

**[Try it now on GitHub Pages](https://aekschen.github.io/gpx-track-replanner)**

## 🎯 How It Works

1. **Load a GPX file** using the "Load GPX" button
2. **Set your starting location** by either:
   - Using "Use My Location" (requires permission)
   - Clicking "Pick on Map" and selecting a point
3. **Click "Replan Route"** to create your loop
4. **Download the result** as a new GPX file

The app will:
- Find the nearest point on your original track
- Route you from your start location to that point
- Include the complete original track
- Route you back to your starting location
- Create a seamless loop

## 🛠️ Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Mapping**: Leaflet.js with OpenTopoMap tiles
- **Routing**: OpenRouteService API
- **Styling**: Custom CSS with dark theme and gradients
- **Deployment**: GitHub Pages

## 📋 Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection for map tiles and routing
- Location permission (optional, for "Use My Location" feature)

## 🔧 Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/aekschen/gpx-track-replanner.git
   cd gpx-track-replanner
   ```

2. **Serve locally** (required for geolocation to work)
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Open in browser**
   ```
   http://localhost:8000
   ```

## 🌍 Deployment to GitHub Pages

1. **Fork or clone** this repository
2. **Rename the HTML file** to `index.html`
3. **Enable GitHub Pages** in repository settings
4. **Your app will be available** at `https://aekschen.github.io/repository-name`

## 🗺️ Map Data Sources

- **Base Maps**: [OpenTopoMap](https://opentopomap.org/) - Topographic maps with hillshading
- **Map Data**: © [OpenStreetMap](https://www.openstreetmap.org/) contributors
- **Elevation Data**: SRTM
- **Routing**: [OpenRouteService](https://openrouteservice.org/)

## 🔐 Privacy & Permissions

- **Location Access**: Only used when you click "Use My Location"
- **No Data Storage**: Your GPX files are processed locally in your browser
- **No Tracking**: No analytics or user tracking implemented
- **API Usage**: Uses OpenRouteService for routing (free tier)

## 🐛 Troubleshooting

### Location Permission Issues
- **Chrome/Edge**: Click the location icon in the address bar and select "Allow"
- **Firefox**: Click the shield icon and enable location sharing
- **Safari**: Check Settings > Privacy & Security > Location Services
- **Alternative**: Use "Pick on Map" instead

### GPX File Issues
- Ensure your file has a `.gpx` extension
- File should contain track points (`<trkpt>` elements)
- Try re-exporting from your GPS device or app

### Routing Issues
- The app uses OpenRouteService's free tier
- If routing fails, it falls back to direct connections
- Large distances may not route properly
- Load in something like komoot to complete routing

## 🤝 Contributing

Contributions are welcome! Here are some ways to help:

- 🐛 Report bugs or issues
- 💡 Suggest new features
- 🔧 Submit pull requests
- 📖 Improve documentation
- 🌍 Add support for new languages

### Development Setup
```bash
# Fork the repo on GitHub
git clone https://github.com/aekschen/gpx-track-replanner.git
cd gpx-track-replanner

# Make your changes
# Test locally
# Submit a pull request
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Leaflet](https://leafletjs.com/) - Amazing mapping library
- [OpenTopoMap](https://opentopomap.org/) - Beautiful topographic tiles
- [OpenRouteService](https://openrouteservice.org/) - Excellent routing API
- [OpenStreetMap](https://www.openstreetmap.org/) - Community-driven map data

## 📧 Support

Having issues? Here are your options:

1. **Check the troubleshooting section** above
2. **Search existing issues** on GitHub
3. **Open a new issue** with details about your problem
4. **Include**: Browser version, error messages, and steps to reproduce

---

**Made with ❤️ for the cycling community**

*Transform any route into the perfect loop starting from your doorstep!*
