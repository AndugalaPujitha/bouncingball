Ball Bounce Detection Using OpenCV
Introduction:
This Python script utilizes the OpenCV library to detect and count the number of bounces made by a ball in a video. It tracks the motion of the ball vertically and identifies instances where it changes direction, indicating a bounce. The script records the count and cumulative time of bounces, displaying the information on the video feed and saving it to a CSV file.
Requirements:
- Python 3.x
- OpenCV (cv2)
- NumPy
- time
- csv

Installation:
Ensure you have Python installed on your system. You can install the required Python libraries using pip:
pip install opencv-python numpy

Input:
- The script requires a video file as input. Update the `cam = cv2.VideoCapture()` line with the path to your video file.
  
Output:
- The script displays the video feed with rectangles drawn around detected circles (representing the ball).
- It shows the count of bounces and the total time of bounces in the video feed.
- Data regarding bounce count and total time is saved to a CSV file named `bounce_data.csv`.

Limitations:
- The script assumes a consistent motion pattern of the ball (vertical bouncing) and may not perform optimally for videos with complex motion or occlusions.
- Accuracy may vary based on lighting conditions, ball size, and background clutter.

