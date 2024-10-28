Here's a sample `README.md` file for your project:

---

# Age Detection App

This is a Python application that uses a trained deep learning model to predict the age group (Young, Middle, or Old) of a detected face in real-time video from a webcam. The app provides a graphical user interface (GUI) using Tkinter and displays the age prediction on the video feed.

## Features

- **Real-Time Face Detection**: Detects faces in the video feed using OpenCV's Haar Cascade Classifier.
- **Age Group Prediction**: Classifies detected faces into age groups using a pre-trained deep learning model.
- **User-Friendly GUI**: Provides an intuitive interface with options to start and stop detection.

## Requirements

- Python 3.6+
- Required libraries (install with pip if necessary):
  - `opencv-python`
  - `numpy`
  - `tensorflow`
  - `Pillow`
  - `tkinter` (usually included with Python on most systems)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/age-detection-app.git
   cd age-detection-app
   ```

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have the following files in the project directory:
   - `model.json`: The JSON file containing the model architecture.
   - `model_weights.weights.h5`: The file with the model's trained weights.

## Usage

1. Run the application:

   ```bash
   python age_detection_app.py
   ```

2. A GUI window will open:
   - Click **Start Detection** to begin age detection.
   - Click **Stop Detection** to stop the video capture.

3. To close the application, simply close the GUI window.

## Code Overview

- **`load_model`**: Loads the model architecture and weights for age prediction.
- **`detect_faces`**: Uses OpenCV's Haar Cascade to detect faces in the video frame.
- **`predict_age`**: Preprocesses detected faces and uses the model to predict the age group.
- **`video_capture_thread`**: Captures video frames in a separate thread for real-time processing.
- **`display_frame`**: Draws bounding boxes around detected faces and displays the age group.

## Troubleshooting

- **Camera Not Detected**: If the camera access fails, ensure that no other application is using it. Restart the app or try reconnecting the webcam.
- **Model Loading Error**: Make sure `model.json` and `model_weights.weights.h5` are available in the directory.

## Dependencies

The `requirements.txt` should contain the following:

```plaintext
opencv-python
numpy
tensorflow
Pillow
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This README provides an overview, installation instructions, usage guide, and troubleshooting tips, making it easier for users to understand and use the application.



# LLM with Digikala Dataset

This project uses a language model (LLM) to answer questions based on Digikala's dataset.

## Installation
Run the following command to install required packages:
```shell
pip install -r requirements.txt
