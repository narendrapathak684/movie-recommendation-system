# Face Recognition System

This project is a Python-based face recognition system that uses OpenCV and deep learning for robust face detection and recognition. It supports both masked and unmasked faces, making it suitable for real-world scenarios such as security, attendance, and identity verification.

## Features

- **Face Detection:** Uses a pre-trained Caffe DNN model for accurate face detection.
- **Face Recognition:** Employs the LBPH algorithm for recognizing faces, even with masks.
- **Dataset Management:** Easily capture and organize images for new users (normal and masked).
- **Training Pipeline:** Simple command-line interface to train the recognizer on your dataset.
- **Real-Time Recognition:** Recognize faces live from your webcam.

## Folder Structure

```
face-recognition-system/
├── face-recog.py              # Main application script
├── deploy.prototxt            # Caffe model architecture for face detection
├── res10_300x300_ssd_iter_140000.caffemodel  # Pre-trained face detection weights
├── face_model.yml             # Trained face recognizer model
├── labels.txt                 # Label mapping for recognized faces
├── dataset/                   # Collected face images
│   └── <person>/
│       ├── normal/            # Images without mask
│       └── masked/            # Images with mask
└── README.md                  # Project documentation
```

## Installation

Install the required dependencies:

```bash
pip install opencv-contrib-python numpy
```

## Usage

Run the main script and follow the menu prompts:

```bash
python face-recog.py
```

1. **Capture:** Collect images for a new person (normal and masked).
2. **Train:** Train the face recognizer on your dataset.
3. **Recognize:** Start real-time face recognition using your webcam.

## Model Files

- `deploy.prototxt` and `res10_300x300_ssd_iter_140000.caffemodel` are required for face detection.
- `face_model.yml` and `labels.txt` are generated after training.

## Notes

- Ensure your webcam is connected and accessible.
- For best results, capture images in good lighting and from multiple angles.

## Author

**narendrapathak684** ([GitHub](https://github.com/narendrapathak684))
