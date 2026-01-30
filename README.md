# License Plate Reader - Real-Time Detection & OCR

A complete, single-file HTML and JavaScript application that uses your webcam and Optical Character Recognition (OCR) to detect and extract license plate numbers in real-time with live visual feedback.

## Features

### Stage 1: Real-Time Detection
- **Live Edge Detection**: Uses Sobel filter to identify high-contrast regions in real-time
- **Contour Analysis**: Identifies rectangular regions with license plate proportions
- **Visual Overlay**: Highlights detected plate regions with green/yellow bounding boxes
- **Aspect Ratio Matching**: Filters regions based on typical plate ratios (1.5:1 to 5.5:1)
- **Adjustable Sensitivity**: Configure edge threshold, min/max area for optimal detection
- **Multi-Candidate Detection**: Identifies up to 3 potential plates per frame

### Stage 2: OCR Processing
- **Smart Cropping**: Automatically crops detected plate region before OCR
- **Tesseract.js Integration**: Powerful OCR engine for text extraction
- **Pattern Recognition**: Intelligent filtering for valid license plate formats
- **Confidence Scoring**: Displays OCR confidence levels with visual indicators
- **Dual Image Display**: Shows both full frame and cropped plate region

### Additional Features
- **Live Webcam Access**: Real-time video feed with camera permission handling
- **Image Capture**: Single-click snapshot with automatic plate region extraction
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **No Backend Required**: Everything runs entirely in the browser
- **Detection Statistics**: Real-time metrics on detection performance
- **Error Handling**: Graceful fallbacks for camera access and processing errors

## Usage

1. Open `license-plate-reader.html` in a modern web browser
2. Allow camera access when prompted
3. Click "Start Detection" to enable real-time plate detection
4. Position a license plate in front of the camera
   - Green boxes indicate detected plate regions
   - Adjust sensitivity settings if needed
5. Click "Capture & Analyze" to take a snapshot and run OCR
6. View the results:
   - Captured full-frame image
   - Cropped license plate region
   - Extracted license plate numbers
   - Confidence scores and detection statistics

## How It Works

### Detection Pipeline
1. **Frame Capture**: Continuously captures video frames at ~10-20 FPS
2. **Grayscale Conversion**: Converts RGB to grayscale for faster processing
3. **Edge Detection**: Applies Sobel filter to detect boundaries and edges
4. **Contour Finding**: Uses flood fill algorithm to identify connected regions
5. **Region Filtering**: Filters by aspect ratio (1.5:1 to 5.5:1) and area
6. **Visual Overlay**: Draws bounding boxes on detected plate regions

### OCR Pipeline
1. **Snapshot**: Captures current video frame
2. **Crop**: Extracts detected plate region with padding
3. **OCR**: Runs Tesseract.js on cropped region (not full frame)
4. **Pattern Matching**: Applies regex patterns to identify license plates
5. **Results**: Displays extracted text with confidence scores

## Settings & Customization

### Detection Settings
- **Edge Threshold** (20-150): Controls sensitivity of edge detection
  - Lower values: More sensitive, detects fainter edges
  - Higher values: Less sensitive, only strong edges
- **Min Area** (500-5000 px²): Minimum size for plate candidates
- **Max Area** (10000-100000 px²): Maximum size for plate candidates

### Tips for Best Results
- **Lighting**: Ensure good, even lighting without harsh shadows
- **Distance**: Keep plate 2-5 feet from camera for optimal focus
- **Angle**: Face the plate directly toward the camera (avoid extreme angles)
- **Contrast**: High-contrast plates (dark text on light background) work best
- **Stability**: Hold plate steady for clearer detection and OCR
- **Settings**: Start with default values, then adjust if needed

## Requirements

- Modern web browser with webcam support (Chrome, Firefox, Safari, Edge)
- Internet connection (for loading Tesseract.js from CDN)
- Camera permissions granted
- HTTPS connection in production (required for camera access)

## Technology Stack

- **HTML5**: Structure, Canvas API for image processing and overlay
- **CSS3**: Modern, responsive styling with gradients and animations
- **JavaScript (ES6+)**: Application logic and computer vision algorithms
- **Tesseract.js**: OCR engine loaded via CDN
- **MediaDevices API**: Webcam access and video streaming
- **Canvas API**: Image capture, edge detection, and visual overlay
- **requestAnimationFrame**: Efficient frame-by-frame processing

## Browser Compatibility

- Chrome/Edge 53+
- Firefox 36+
- Safari 11+
- Opera 40+

## Performance

- **Detection**: ~10-20 FPS on modern devices
- **Edge Detection**: ~50-100ms per frame at 720p
- **OCR Processing**: ~2-5 seconds for typical license plate
- **Memory Usage**: ~50-100MB for video and processing

## Privacy & Security

All processing happens locally in your browser:
- No images sent to external servers
- No data collection or tracking
- Camera stream remains on your device
- Images exist only in browser memory during processing
- Proper cleanup when page is closed

## Troubleshooting

### Camera Access Issues
- Ensure you've granted camera permissions in browser settings
- Check that no other application is using the camera
- Refresh the page and allow permissions when prompted
- Use HTTPS (not HTTP) for camera access

### Detection Not Working
- Adjust edge threshold (try lower values for subtle plates)
- Increase min area if detecting too many false positives
- Ensure good lighting without glare or reflections
- Try different angles and distances

### Low OCR Accuracy
- Improve lighting conditions
- Ensure plate is in focus and clearly visible
- Clean the license plate if dirty or damaged
- Try capturing when plate is centered in green box
- Verify detection settings are appropriate for plate size

## Development

This is a self-contained single-file application. To modify:
1. Open `license-plate-reader.html` in a text editor
2. JavaScript is embedded in `<script>` tags
3. CSS is embedded in `<style>` tags
4. No build process or compilation required
5. Refresh browser to see changes

## License

This project is open source and available for educational and personal use.

## Acknowledgments

- **Tesseract.js**: OCR engine for text extraction
- **Sobel Filter**: Classic edge detection algorithm
- **MediaDevices API**: Web standard for camera access
