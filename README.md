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

## License

MIT License

---

```
MIT License

Copyright (c) 2025 Prabesh Pathak

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```