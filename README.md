# PushUpCounter
# StayFit with Abdul - Push-Up Counter

StayFit with Abdul is a cutting-edge Python program designed to revolutionize the way individuals track their push-up workouts. Leveraging the power of Mediapipe and OpenCV technologies, this program offers a simple yet effective solution for counting push-ups accurately while ensuring proper form.

## Features

- **Push-Up Counting:** Accurately counts the number of push-ups performed by the user in real-time.
- **Form Feedback:** Provides instant feedback on form and posture, helping users maintain proper alignment and technique.
- **Visual Representation:** Utilizes Mediapipe's Pose module to detect key body landmarks, providing users with a visual representation of their push-up performance.
- **Customizable:** The BasicPoseModule can be easily adapted and integrated into personal projects, with adjustable variables and parameters to suit individual preferences.

## How It Works

1. **Pose Detection:** The program utilizes Mediapipe's Pose module to detect key body landmarks, including shoulders, elbows, and hips, in real-time.
2. **Push-Up Tracking:** By analyzing the user's body movements, the program accurately counts the number of push-ups completed, providing instant feedback on progress.
3. **Form Feedback:** Visual cues and indicators guide users to maintain proper form and alignment throughout their push-up workout, ensuring maximum effectiveness and safety.

## Usage

To use StayFit with Abdul in your projects, simply integrate the BasicPoseModule and adjust variables as necessary. Refer to the included documentation for detailed instructions on customization and implementation.

```python
from BasicPoseModule import PoseModule

# Initialize Pose Module
pose = PoseModule()

# Main loop
while True:
    # Get frame from camera
    frame = capture_frame()
    
    # Perform pose detection
    landmarks = pose.detect_landmarks(frame)
    
    # Count push-ups and provide feedback
    push_up_count = pose.count_push_ups(landmarks)
    pose.display_feedback(frame, push_up_count)
```

![](https://github.com/Abdul-Rehman-Astro/Pushups_by_Abdul/blob/main/Images/Pushup%20counter.png)
![](https://github.com/Abdul-Rehman-Astro/Pushups_by_Abdul/blob/main/Images/Pushup%20counter%202.png)

![alt text](https://google.github.io/mediapipe/images/mobile/pose_tracking_full_body_landmarks.png)

