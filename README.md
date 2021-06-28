# Facial landmarks Detection using dlib, OpenCV, and Python

<ul>
<li> Eyes </li>
<li> Eyebrows </li>
<li> Nose </li>
<li> Mouth </li>
<li> Jawline </li>
</ul>

## What are facial landmarks?

<p >Detecting facial landmarks is a subset of the shape prediction problem. Given an input image (and normally an ROI that specifies the object of interest), a shape predictor attempts to localize key points of interest along the shape. </p>
 <img src="facial_landmarks.jpg" width="30%">

 ## Understanding dlib’s facial landmark detector
 <p> The pre-trained facial landmark detector inside the dlib library is used to estimate the location of 68 (x, y)-coordinates that map to facial structures on the face.

The indexes of the 68 coordinates can be visualized on the image below:</p>

<img src="facial_landmarks_68_coordinates.jpg" width="30%">

<p> These annotations are part of the 68 point iBUG 300-W dataset which the dlib facial landmark predictor was trained on.

It’s important to note that other flavors of facial landmark detectors exist, including the 194 point model that can be trained on the HELEN dataset.

Regardless of which dataset is used, the same dlib framework can be leveraged to train a shape predictor on the input training data, this is useful if you would like to train facial landmark detectors or custom shape predictors of your own.</p>
