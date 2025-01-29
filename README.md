# AR Experience

An interactive web-based Augmented Reality application that allows users to project screen shares and images onto AR markers in real-time.

## 🌟 Features

- **Screen Share AR**
  - Project your screen content in augmented reality
  - Real-time screen capture and display
  - Seamless integration with AR markers

- **Image Upload AR**
  - Upload and display images in AR space
  - Background removal capability
  - Interactive image positioning

- **Capture Functionality**
  - Screenshot capability for AR scenes
  - Flash effect for capture feedback
  - Automatic image download

## 🚀 Technologies Used

- A-Frame (v1.2.0) - WebVR framework
- AR.js - Augmented Reality library
- HTML5 Canvas API
- WebRTC for screen sharing
- Remove.bg API for background removal

## 📋 Prerequisites

- Modern web browser (Chrome, Firefox, or Edge recommended)
- Webcam or device camera
- Internet connection
- Local web server for development

## 💻 Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd ar-experience
```

2. Set up the local development server:
```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000
```

3. Access the application:
```
http://localhost:8000
```

## 🛠️ Configuration

### Remove.bg API Setup
1. Sign up at [Remove.bg](https://www.remove.bg/api)
2. Get your API key
3. Replace the API key in `script.js`:
```javascript
headers: {
  'X-Api-Key': 'your-api-key-here'
}
```

### AR Marker Setup
1. Visit [AR.js Marker Training](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html)
2. Generate your marker pattern
3. Save as `pattern-Batman.patt` in project root

## 📱 Usage

### Screen Share AR
1. Navigate to "Screen Share AR"
2. Click "Start Screen Share"
3. Select screen/window to share
4. Show AR marker to camera
5. Use "Capture Screen" to project

### Image Upload AR
1. Navigate to "Image Upload AR"
2. Upload an image
3. Show AR marker to camera
4. Optionally remove background
5. Capture scene using shutter button

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👥 Development Team

- Nagaraju P
- Nandan M N
- Amith H Nithyundil
- Akash Ravindra Nilkund

Under the guidance of:
Mr. DEEPAK P
Assistant Professor
Dept. of CS & Engineering
NIEIT, Mysore

## 🔧 Troubleshooting

### Common Issues:
1. **Camera Access Denied**
   - Grant camera permissions in browser settings
   - Ensure camera isn't in use by other applications

2. **AR Marker Not Detected**
   - Improve lighting conditions
   - Keep marker flat and fully visible
   - Maintain optimal distance from camera

3. **Screen Share Not Working**
   - Use compatible browser
   - Grant screen sharing permissions
   - Try sharing specific window instead of entire screen

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🔮 Future Enhancements

- Multiple AR marker support
- Real-time video streaming in AR
- Custom marker upload functionality
- Mobile app integration
- Cloud storage for AR content
- Collaborative AR features

## 💡 Browser Support

- Chrome 76+
- Firefox 68+
- Edge 79+
- Safari 13+ (limited AR support)

## ⚠️ Important Notes

- HTTPS required for camera access when hosted online
- HTTP works for localhost development
- Mobile devices require WebGL and gyroscope support
- API key required for background removal feature
