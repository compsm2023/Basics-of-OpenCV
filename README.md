# Webcam Filters based on OpenCV

A real-time webcam filter application built with OpenCV that allows you to apply various image filters and effects to your webcam feed using keyboard shortcuts.

## Features

This application provides the following filter modes:

- **Normal Mode** - Standard webcam view
- **Grayscale Filter** - Converts the video feed to grayscale
- **Gaussian Blur** - Applies a blur effect to the video
- **Edge Detection** - Detects and highlights edges using Canny edge detection
- **Horizontal Flip** - Mirrors the video horizontally

## Requirements

- Python 3.x
- OpenCV (cv2) library
- Webcam/camera device

## Installation

1. Install OpenCV using pip:
```bash
pip install opencv-python
```

## Usage

1. Run the script:
```bash
python webcam_filters.py
```

2. Use the following keyboard shortcuts to switch between filters:
   - **'n'** - Normal mode (default)
   - **'g'** - Grayscale filter
   - **'b'** - Gaussian Blur
   - **'e'** - Edge Detection
   - **'f'** - Horizontal Flip
   - **'q'** - Quit the application

## How It Works

The application captures video frames from your default webcam (camera index 0) and applies real-time filters based on the selected mode. Each filter mode processes the frame differently:

- **Grayscale**: Converts BGR color space to grayscale
- **Gaussian Blur**: Applies a 21x21 Gaussian blur kernel
- **Edge Detection**: Converts to grayscale, applies blur, then uses Canny edge detection
- **Horizontal Flip**: Mirrors the frame along the vertical axis

## Notes

- Make sure your webcam is connected and not being used by another application
- The application displays filter mode indicators on the video feed
- Press 'q' to quit and release the camera resources

## Author

compsm2023

## License

This project is open source and available for educational purposes.
