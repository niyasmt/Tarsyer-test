# Readme

# Hand Tracking

# Requirements
python <br>
Open CV <br>
MediaPipe <br>

# Mediapipe
MediaPipe is a framework mainly used for building audio, video, or any time series data. With the help of the MediaPipe framework, we can build very impressive pipelines for different media processing functions.

Some of the major applications of MediaPipe.

Multi-hand Tracking
Face Detection
Object Detection and Tracking etc

# Hand Landmark Model

<img src = "https://github.com/niyasmt/Tarsyer/blob/main/Image/Hand.png" width = "700" hight = "500"/>

# MediaPipe Holistic
Mediapipe Holistic is one of the pipelines which contains optimized face, hands, and pose components which allows for holistic tracking, thus enabling the model to simultaneously detect hand and body poses along with face landmarks. one of the main usages of MediaPipe holistic is to detect face and hands and extract key points to pass on to a computer vision model.

Output Vedio <br>
https://github.com/niyasmt/Tarsyer/blob/main/Image/Facial%20and%20Hand%20Landmarks%202022-08-19%2013-56-36.mp4 <br>

Source Code <br>
https://github.com/niyasmt/Tarsyer/blob/main/Hand_tracking.py <br>

# Click and Crop image

You can easily crop an image using mouse clicks on OpenCV. For this you need call the OpenCV cv2.setMouseCallback(“window”, image). <br>
You then need to detect the left mouse button down using the cv2.EVENT_LBUTTONDOWN event, <br>
then continuously locate the position of the mouse using the cv2.EVENT_MOUSEMOVE event and at last you need to detect the left mouse button released or cv2.EVENT_LBUTTONUP event.

Source Code <br>
https://github.com/niyasmt/Tarsyer/blob/main/Image_cropping.py

# Morphological Operations
Python OpenCV Morphological operations are one of the Image processing techniques that processes image based on shape. This processing strategy is usually performed on binary images. <br.
<br>
# Morphological operations based on OpenCV are as follows
Erosion <br>
Dilation <br>
Opening <br>
Closing <br>

# Erosion
It erods away the boundaries of forground object <br>
Erosion primarily involves eroding the outer surface (the foreground) of the image. As binary images only contain two pixels 0 and 255, it primarily involves eroding the foreground of the image and it is suggested to have the foreground as white. The thickness of erosion depends on the size and shape of the defined kernel. We can make use of NumPy’s ones() function to define a kernel. <br><br>

# Dilation
Purifying the image <br>
Dilation involves dilating the outer surface (the foreground) of the image. As binary images only contain two pixels 0 and 255, it primarily involves expanding the foreground of the image and it is suggested to have the foreground as white. The thickness of erosion depends on the size and shape of the defined kernel. We can make use of NumPy’s ones() function to define a kernel. <br><br>

Source Code <br>
https://github.com/niyasmt/Tarsyer/blob/main/Morphological_trasformation.py <br><br>

# Thresholding <br>
Thresholding is a technique in OpenCV, which is the assignment of pixel values in relation to the threshold value provided. In thresholding, each pixel value is compared with the threshold value. If the pixel value is smaller than the threshold, it is set to 0, otherwise, it is set to a maximum value (generally 255). Thresholding is a very popular segmentation technique, used for separating an object considered as a foreground from its background <br>
Source Code <br>
https://github.com/niyasmt/Tarsyer/blob/main/Tresholding.py
