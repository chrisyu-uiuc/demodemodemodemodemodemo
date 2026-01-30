# License Plate Detection & Recognition System

A modern, browser-based license plate detection and recognition system built with JavaScript, OpenCV.js, and Tesseract.js.

## Features

- **Multiple Input Methods**
  - Drag & drop image upload
  - Click to select image files
  - Live camera capture

- **Image Preprocessing**
  - Grayscale conversion
  - Gaussian blur for noise reduction
  - Contrast enhancement
  - Adaptive thresholding
  - Morphological operations (opening/closing)
  - Contour detection for plate region identification

- **OCR Recognition**
  - Powered by Tesseract.js
  - Multi-language support (English, German, French, Spanish)
  - Confidence score calculation

- **User Interface**
  - Modern, responsive dark theme
  - Real-time processing indicators
  - Results display with confidence visualization
  - Detection history with timestamps
  - Adjustable preprocessing parameters

## Usage

1. **Open the Application**
   - Simply open `index.html` in a modern web browser (Chrome, Firefox, Edge, Safari)

2. **Select an Input Method**
   - **Upload**: Drag & drop an image or click to select a file
   - **Camera**: Click "Open Camera" to access your device's camera (requires HTTPS or localhost)

3. **Process the Image**
   - Click "Detect Plate" to analyze the image
   - The system will:
     - Preprocess the image to enhance plate visibility
     - Extract potential license plate regions
     - Perform OCR to read the text
     - Display results with confidence scores

4. **Adjust Settings (Optional)**
   - **OCR Language**: Select the appropriate language for better recognition
   - **Contrast Enhancement**: Adjust contrast (0-100) to improve plate visibility
   - **Threshold Value**: Modify thresholding (0-255) for different lighting conditions

## Technical Details

### Dependencies

- **OpenCV.js** (4.8.0): Image processing and computer vision
- **Tesseract.js** (v5): Optical character recognition
- **Modern Web APIs**: Camera access, File API, Canvas API

### Image Processing Pipeline

1. Load image into canvas
2. Convert to grayscale
3. Apply Gaussian blur
4. Enhance contrast
5. Apply adaptive thresholding
6. Perform morphological operations
7. Detect contours
8. Extract regions of interest
9. Perform OCR on detected regions

### Browser Requirements

- Modern browser with JavaScript enabled
- Camera access requires HTTPS or localhost
- WebAssembly support (for OpenCV.js)
- Approximately 50-100 MB available memory for processing

## Performance Tips

- For best results, use images with good lighting
- License plates should be clearly visible and not heavily distorted
- The system works best with standard license plate formats
- Processing time varies by image size and complexity (typically 1-5 seconds)

## Limitations

- Accuracy depends on image quality and lighting conditions
- May struggle with heavily damaged or obscured plates
- Performance can vary based on device capabilities
- Requires internet connection for loading CDN resources

## License

This project is provided as-is for educational and demonstration purposes.
