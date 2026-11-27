# Vision-Guided-Robot-Manipulation
Vision-guided robotic manipulation using a Techman TM5 collaborative robot, integrating ML-based object detection, coordinate transformations, and automated pick-and-place tasks.
## Vision-Guided Candy Sorting with a TM5 Collaborative Robot

Built an automated pick-and-place system that sorts milk and lemon candies using a TM5 collaborative robot and its built-in camera.

- Trained a TM AI+ object detection model to distinguish milk candies from lemon candies. When multiple candies appeared in the camera view, the system selected the detection with the highest confidence score and checked whether its class still needed more pieces before picking it up. Target counts were configurable by class, such as seven milk candies and nine lemon candies.

- Designed a modular TMflow workflow that combined vision-based pick coordinates with robot-frame waypoints and voltage-based gripper control.

- Used the Techman Robot logo between two connected bins as a visual landmark. The robot located each bin opening relative to the landmark, allowing it to place candies into the correct bin even when the bin assembly was rotated.


### Experimental Demonstration
https://github.com/user-attachments/assets/7f9b3000-ce5c-4464-952e-bd925ff56dcd

## Gemini-Powered Object Recognition with OpenCV Foreground Extraction

Developed an object recognition pipeline that uses OpenCV to extract foreground objects from camera images and sends the extracted regions to a multimodal model through the Gemini API. The model returns semantic descriptions of the observed objects, enabling recognition across different object categories without training or fine-tuning a task-specific recognition model.

https://github.com/user-attachments/assets/5da7013a-e2a9-4a0d-a44d-53191cf0349a


## Gemini-Assisted Vision-Guided Grasping with a TM5 Collaborative Robot

Extended the recognition pipeline to robotic grasping by combining Gemini-based object identification with vision-based object localization. A calibration board establishes the mapping between image coordinates and the robot-base coordinate frame, allowing the Techman TM5 collaborative robot to move to the identified object's location and execute a grasp.

https://github.com/user-attachments/assets/39737258-43ca-44bf-8ccb-7fc759fdc8d3



