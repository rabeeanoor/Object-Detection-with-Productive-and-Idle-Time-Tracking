
# Video Object Detection with Productive and Idle Time Tracking

This Python script utilizes YOLOv5 for object detection in a video feed. Additionally, it tracks the productive and idle time of individuals within a region of interest (ROI) defined in the video.

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- PyTorch
- NumPy
- tqdm
- Matplotlib

## Installation

You can install the required packages via pip:

```bash
pip install torch torchvision
pip install opencv-python tqdm matplotlib
```

## Usage

1. Ensure you have the necessary dependencies installed.
2. Place your video file in the same directory as the script or provide the path to the video file.
3. Update the `file` variable with the name of your video file.
4. Run the script. It will perform object detection on the video frames, drawing bounding boxes around detected persons. It also calculates and overlays productive and idle times.
5. Press 'q' to exit the video feed.

## Output

The script will generate an output video file named `output_video.mp4` in the same directory as the script. Additionally, it will save images of detected persons within the ROI, named `detected_person_x.jpg`, where `x` represents the frame number.

## Notes

- Adjust the confidence threshold (`model.conf`) and other parameters as needed.
- Modify the ROI points (`points`) as required for your video.
- The script assumes a constant frame rate for the video. If the frame rate varies, adjust the calculations accordingly.
