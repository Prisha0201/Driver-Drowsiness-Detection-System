# Drowsiness Detection System

A real-time webcam application that uses OpenCV and dlib facial landmarks to identify closed or partially closed eyes. The current status is drawn on the camera feed as `Active`, `Drowsy`, or `SLEEPING`.

## Requirements

- Windows with Python 3.10 recommended
- A working webcam
- `opencv-python`, `numpy`, `dlib`, and `imutils`
- The dlib 68-point facial landmark model

## Setup

1. Create and activate a virtual environment:

	```powershell
	python -m venv myenv
	.\myenv\Scripts\Activate.ps1
	```

2. Install the Python packages:

	```powershell
	python -m pip install opencv-python numpy dlib imutils
	```

3. Download `shape_predictor_68_face_landmarks.dat` from the [dlib model downloads](http://dlib.net/files/) page. Extract it and place the `.dat` file in this project directory, beside `drowniness.py`.

## Run

From the project directory, run:

```powershell
python .\drowniness.py
```

The application opens the default webcam. Press `Esc` to stop it.

## Notes

- Make sure no other application is using the webcam.
- The script currently opens camera index `0`; change `cv2.VideoCapture(0)` if a different camera is required.
- This is an assistive prototype, not a certified driver-safety system. Do not rely on it as the only protection against drowsy driving.
