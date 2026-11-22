# Vision-Guided-Robot-Manipulation
Vision-guided robotic manipulation using a Techman TM5 collaborative robot, integrating ML-based object detection, coordinate transformations, and automated pick-and-place tasks.
## Vision-Guided Candy Sorting with a TM5 Collaborative Robot

Built an automated pick-and-place system that sorts milk and lemon candies using a TM5 collaborative robot and its built-in camera.

- Trained a TM AI+ object detection model to distinguish milk candies from lemon candies. When multiple candies appeared in the camera view, the system selected the detection with the highest confidence score and checked whether its class still needed more pieces before picking it up. Target counts were configurable by class, such as seven milk candies and nine lemon candies.

- Designed a modular TMflow workflow that combined vision-based pick coordinates with robot-frame waypoints and voltage-based gripper control.

- Used the Techman Robot logo between two connected bins as a visual landmark. The robot located each bin opening relative to the landmark, allowing it to place candies into the correct bin even when the bin assembly was rotated.


### Experimental Demonstration
https://github.com/user-attachments/assets/7f9b3000-ce5c-4464-952e-bd925ff56dcd





