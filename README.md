# License Plate Reader - Webcam OCR Application

A complete, single-file HTML and JavaScript application that uses your webcam and Optical Character Recognition (OCR) to detect and extract license plate numbers in real-time.

## Features

- **Live Webcam Access**: Access and display your device's camera feed in real-time
- **Image Capture**: Take snapshots of the video stream with a single click
- **OCR Processing**: Uses Tesseract.js to extract text from captured images
- **License Plate Detection**: Intelligent pattern matching to identify license plate numbers
- **Confidence Scoring**: Displays OCR confidence levels with visual indicators
- **Responsive Design**: Works on desktop and mobile devices
- **No Backend Required**: Everything runs entirely in the browser

## Usage

1. Open `license-plate-reader.html` in a modern web browser
2. Allow camera access when prompted
3. Position a license plate in front of the camera
4. Click "Capture & Analyze" to take a snapshot and analyze it
5. View the detected license plates and confidence scores

## Requirements

- Modern web browser with webcam support (Chrome, Firefox, Safari, Edge)
- Internet connection (for loading Tesseract.js from CDN)
- Camera permissions granted

## Tips for Best Results

- Ensure good lighting conditions
- Keep the license plate centered and clearly visible
- Avoid reflections and glare on the plate
- Maintain a reasonable distance for optimal focus
- Use high-contrast plates for better OCR accuracy

## Technology Stack

- **HTML5**: Structure and Canvas API for image capture
- **CSS3**: Modern, responsive styling with gradients and animations
- **JavaScript (ES6+)**: Application logic and webcam handling
- **Tesseract.js**: OCR engine loaded via CDN
- **MediaDevices API**: Webcam access and video streaming

## Browser Compatibility

- Chrome/Edge 53+
- Firefox 36+
- Safari 11+
- Opera 40+

## Privacy

All processing happens locally in your browser. No images or data are sent to any server.

## License

This project is open source and available for educational and personal use.
