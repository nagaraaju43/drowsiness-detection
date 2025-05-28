

This program is used to detect drowsiness for any given person. In this program we check how long a person's eyes have been closed for. If the eyes have been closed for a long period i.e. beyond a certain threshold value, the program will alert the user by playing an alarm sound.

The program contains 3 files, which are
## Files
 - **face_and_eye_detector_single_image.py** - Detects face and eye from a single image.
 Demo-
 
|  ![Test Image](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/test.jpeg)| ![Result Image](https://github.com/mohitwildbeast/Driver-Drowsiness-Detector/blob/master/images/result_face_detector_single_image.png) |
|---|---|
 
 ## Requirements
> 
> IMPORTANT

  Download `shape_predictor_68_face_landmarks.dat.bz2` from [Shape Predictor 68 features](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) 
  Extract the file in the project folder using 
  ``bzip2 -dk shape_predictor_68_face_landmarks.dat.bz2``


    numpy==1.23.5
	dlib==19.24.0
	pygame==2.1.3
	imutils==0.5.4
	opencv-python==4.9.0.80
	scipy==1.10.1

Use `pip install -r requirements.txt`to install the given requirements.

## Usage

### Detect Face and Eyes in a Single Image
Put your file to be detected in **images** folder with name **test.jpeg** or change the file path in `Line : 14 face_and_eye_detector_single_image.py` to your image file.                     
Run script using:

    python face_and_eye_detector_single_image.py

### Detect Face and Eyes in a Webcam Feed
Run script using:

    python face_and_eye_detector_webcam_video.py
### Drowsiness Detection
Run script using:

    python drowsiness_detect.py

The algorithm for Eye Aspect Ratio was taken from pyimagesearch.com blog, by Adrian RoseBrock.
