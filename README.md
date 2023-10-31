<h1><center>Robust Human Target Detection and Acquisition</center></h1>
<h2><center>Team: Slow Code Transform</center></h2>
<h2><center>Indian Institute of Technology Kharagpur</center></h2>

<h2> Details of Radar Image Processing </h2>
The radar signals are first processed using a traditional micro-doppler radar signal processing pipeline and then passed through an 
<br>LSTM supported CNN model to detect and classify the Human Activities. Human Activity Recoginition and Classification is done using a VGG19 Model. The CNN model classifies the activities into:

<UL>
  <li>Crawling</li>
  <li>Jumping (includes the possibility of weapons)</li>
  <li>Running/Jogging</li>
  <li>Walking/Marching</li>
  <li>Stone-pelting/Grenade throwing</li>
</UL>

Detailed CNN Architecture for suspicious activity classification using μ-Doppler Radar Images:
<img src = "https://github.com/zaid-24/College-Work/blob/main/Radar%20Image%20Processing/images/classification%20model.png">
<i>Source: S.V. Dhavale et. al, Application of DNN for radar micro-doppler signature-based human
suspicious activity recognition, Pattern Recognition Letters-2022</i>

<br> This CNN Architecture is a part of a bigger network:

<img src = "https://github.com/zaid-24/College-Work/blob/main/Radar%20Image%20Processing/images/pipeline.png">
<i>Source: Zhaoyue Wang, Chao Yang et. al, Radar Human Activity Recognition with an Attention-Based
Deep Learning Network, Sensors-2023</i>
<br><br>
The CNN model architecture uploaded on the repository is designed using <a src="https://www.tensorflow.org/">Tensorflow</a> and is trained on
<br>the dataset: <a src = "https://ieee-dataport.org/documents/diat-%CE%BCradhar-radar-micro-doppler-signature-dataset-human-suspicious-activity-recognition"> <b>DIAT-μ RadHAR (Micro-Doppler Signature Dataset) </b> </a> available at <a src="https://ieee-dataport.org/"> <b>IEEE Dataport </b> </a> 


<h2>Details of Activity Recognition</h2>
<p>This project focuses on real-time activity recognition using computer vision and deep learning techniques. It utilizes the YOLO (You Only Look Once) object detection model to identify and classify objects of interest in a video stream. The primary goal is to detect suspicious activities by recognising specific objects within the video frames.</p>

<p>The project uses YOLO object detection for real-time video analysis. It has predefined classes for alerting based on the objects detected in the video frames:</p>

<ul>
  <li>People</li>
  <li>Car</li>
  <li>Truck</li>
  <li>Backpack</li>
  <li>Suspicious handheld device</li>
  <li>Handbag</li>
  <li>Suitcase</li>
</ul>

<p>The code performs the following steps:</p>

<ul>
    <li>Initializes the YOLO model with the provided weights.</li>
    <li>Opens the video file.</li>
    <li>Processes each frame of the video.</li>
    <li>Detects and classifies objects in the frames.</li>
    <li>Alerts if any alerting classes are detected in the frame, displaying the reasons for the alert in the image.</li>
    <li>Continues processing frames until the video ends.</li>
  </ul>

  <p>The code displays an "ALERT!" message on the video frame if any alerting objects are detected. It also lists the reasons for the alert, indicating which objects triggered the alert.</p>
  