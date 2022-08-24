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

<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/Hand.png" width = "700" hight = "500"/>

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

# People Counting 
# CSRNET Model
for Congested Scene Recognition called CSRNet to provide a data-driven and deep learning method that can understand highly congested scenes and perform accurate count estimation as well as present high-quality density maps. The proposed CSRNet is composed of two major components: a convolutional neural network (CNN) as the front-end for 2D feature extraction and a dilated CNN for the back-end. Trained with shanghai dataset<br>

# SSD
Single Shot MultiBox Detector <br>
Trained with coco dataset <br>
SSD is a state-of-the-art object detection algorithm that achieves similar or even higher accuracy than Faster R-CNN.
<br>
Source code <br>
https://github.com/niyasmt/Tarsyer-test/blob/master/people%20counting%20using%20ssd.ipynb

# YOLOv5
You Only Look Once <br>
Trained with coco128 dataset <br>
This approach uses a single neural network to process the entire picture, then separates it into parts and predicts bounding boxes and probabilities for each component. These bounding boxes are weighted by the expected probability. The method “just looks once” at the image in the sense that it makes predictions after only one forward propagation run through the neural network. It then delivers detected items after non-max suppression. <br>

Source Code<br>
https://github.com/niyasmt/Tarsyer-test/blob/master/People%20counting%20using%20yolov5.ipynb

# Comparison of Three Model
Add a picture that include 9 people<br>
<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/crowd.jpg" width = "700" hight = "500"/> <br>
Output<br>

CSRNET  : 27 people<br>
SSD     : 7 people<br><br>
<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/download%20(1).png" width = "700" hight = "500"/> <br>
YOLOv5  : 16 People<br><br>
<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/yolo%20small.jpg" width = "700" hight = "500"/> <br>

Add a picture that include 50 people<br>
<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/50.jpg" width = "700" hight = "500"/> <br>
Output<br>

CSRNET  : 47 people<br>
SSD     : 11 people<br><br>
<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/download.png" width = "700" hight = "500"/> <br>
YOLOv5  : 31 People<br><br>
<img src = "https://github.com/niyasmt/Tarsyer-test/blob/master/Images/Yolo%20crowd.jpg" width = "700" hight = "500"/> <br>


# Conclusion
More congested images CRNET is work very good <br>
Small Crowd images SSD is work very good <br>




