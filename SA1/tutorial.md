Open Camera
============


In this activity, you will learn to open the camera on your device using .




<img src= "https://media.slid.es/uploads/1525749/images/10509559/SA1.png" width = "480" height = "320">




Follow the given steps to complete this activity:
1. Open camera and capture the video


* Open file main.py.


* Import cv2 library.


  `import cv2`


* Capture the camera feed using `cv2.VideoCapture(0)` and set the resolution using `cap.set()` function.


  `cap = cv2.VideoCapture(0)`


  `cap.set(3, 1280)`


  `cap.set(4, 720)`


2. Read the video


* Use the while loop to display the video.


  `while True:`


* Write a try-except block in the while loop.


 
    `try:`
   
    `except Exception as e:`
        `print(e)`


* Read the video using `cap.read()` method.


  `readVideo = cap.read()`


* Get the first frame of the video by `readVideo[0]`.
  `check = readVideo[0]`


* Get the camera feed by getting the second frmae by `readVideo[1]` and store in variav.


  `cameraFeedImg= readVideo[1]`


* Flip the camera by using `cv2.flip()` and pass the cameraFeedImg to it.
  `cameraFeedImg = cv2.flip(cameraFeedImg, 1)`


* Save and run the code to check the output.
