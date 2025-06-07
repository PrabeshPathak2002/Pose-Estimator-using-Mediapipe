# Pose Estimator using Mediapipe and OpenCV

This project demonstrates human pose estimation in videos or webcam streams using [Mediapipe](https://mediapipe.dev/) and [OpenCV](https://opencv.org/) in Python.

## Features

- Real-time pose detection and landmark tracking
- Works with both video files and webcam input
- Easily extract and use specific pose landmarks
- FPS display on video feed
- Modular, class-based code

## Requirements

- Python 3.7+
- opencv-python
- mediapipe

Install dependencies with:

```sh
pip install -r requirements.txt
```

## Usage
To run pose estimation on a video file:

```python
python PoseEstimatorModule.py
```
Edit the `main()` function in `PoseEstimatorModule.py` to set your video file path, for example:

```python
pose_estimator = PoseEstimator(video_path="PoseVideos/1.mp4")
```

To use your webcam, leave `video_path` as  `None`:

```python
pose_estimator = PoseEstimator()
```

## Customization

- To extract specific landmarks, use the `get_position` method and provide landmark IDs.
- To change video resolution, use `cv2.resize()` after reading each frame in the code.

## File Structure

- `PoseEstimatorModule.py` – Main class-based pose estimation module.
- `PoseVideos/` – Folder for sample video files.
- `requirements.txt` – Python dependencies.
- `.gitignore` – Files and folders to ignore in git.

## Screenshot
![alt text](https://github.com/PrabeshPathak2002/Pose-Estimator-using-Mediapipe/blob/main/Screenshot.png "Screenshot")

## Pose Landmarks
![alt text]([https://github.com/PrabeshPathak2002/Pose-Estimator-using-Mediapipe/blob/main/Screenshot.png](https://www.researchgate.net/publication/372215767/figure/fig1/AS:11431281173353112@1688826988871/Mediapipe-Pose-landmarks.png) "Landmarks")
