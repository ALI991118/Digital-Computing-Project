# **Yoga Pose Classification and Evaluation Project**

github link: https://github.com/ALI991118/Digital-Computing-Project.git

### **Description**

This project utilizes Computer Vision and Machine Learning techniques to recognize and evaluate yoga poses in real-time using the MediaPipe framework. It involves analyzing body angles to classify different yoga poses and provide feedback on the accuracy of the user's pose.



### **Project Structure**

- `model_angle.ipynb` : 

​	Calculates the angles between joints to define and recognize yoga poses.

- `yoga_trainer.ipynb` :

​	Integrates the pose recognition with real-time video capture to evaluate and give feedback on user performance.

- `dataset`: 

  Contains images used for training and testing the angle calculations for different yoga poses. 

  This includes:

  - `t_pose/`: Images for T Pose recognition.
  - `tree_pose/`: Images for Tree Pose recognition.

​		



### **Setup**

#### **Prerequisites**

- Python 3.6-3.9
- OpenCV Library
- MediaPipe
- Numpy

#### Installation

1. Clone this repository to your local machine.

2. Ensure you have Python installed, then set up a virtual environment:

   ```
   python -m venv yoga-env
   source yoga-env/bin/activate  # On Windows use yoga-env\Scripts\activate
   ```

3. Install the required packages:

   ```
   pip install opencv-python-headless mediapipe numpy
   ```

#### Running the Notebooks

1. Open the notebooks using Jupyter Notebook or JupyterLab:

```
jupyter notebook
```

2. Run `model_angle.ipynb` to see how angles are calculated between joints.

3. Execute `yoga_trainer.ipynb` to start the real-time pose recognition and evaluation.





### How It Works

- **Angle Calculation**: The `model_angle.ipynb` notebook demonstrates how to calculate angles using the keypoints detected by MediaPipe. This is fundamental in defining what constitutes a specific yoga pose.
- **Real-time Feedback**: The `yoga_trainer.ipynb` uses the camera feed to detect a user's pose, calculates angles, and compares these with predefined pose angles to give real-time feedback.