# **Name**
Drowsiness Detector
Python model to detect the drowsiness of the Driver.

# **Description**
This model has following key steps:
	- It detects the human face for the live vedio by processing each frame.
	- Then with the help of dlib library of python and a dataset file we get the location of points on the face.
	- After this it calculates the eye aspect ratio to get how much the eye of the person is open.
	- This process continues till the aspect ratio is smaller than a desired one for particular frames.
	- On encountering above condition the alert is raised  

# **Prerequisites**
`Pyhton3` installed with following libraries on your system.

# **Libraries needed**
1. `scipy` to compute the Euclidean distance between facial landmark points in the eye aspect ratio.
    - `Install` with following command `pip install scipy`
2. `imutils` for vedio and image processing
    - `Install` with following command `pip install imutils` 
3. `thread` for playing alert without intrupting or pausing the script
    - `Install` with following command `pip install threaded`
4. `playsound` for playing alert
    - `Install` with following command `pip install playsound`
5. `dlib` most important of all for returning the facial points
    - `Install` with following command `pip install dlib` and make sure you have cmake installed.
6. `cv2` and `numpy` for computer vision on images
    - `Install` with following command `pip install opencv-python` and `pip install numpy`

# **How to run** 
After the installation of all packages run with the following command
`python detect_drowsiness.py \--shape-predictor face_shape_predictor.dat \--alarm alert.wav`

# **Disclaimer**
This project was by me to detect drowsiness in drivers and raise a appropriate alert so as to minimise road accidents due to drowsiness.