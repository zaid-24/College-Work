# College-Work
<h1>Robust Human Target Detection and Acquisition</h1>
<h2>Team: Slow Code Transform</h2>
<h2>Indian Institute of Technology Kharagpur</h2>

<h2> Details of Radar Image Processing </h2>h2>
The radar signals are first processed using a traditional micro-doppler radar signal processing pipeline and then passed through an 
<br>LSTM supported CNN model to detect and classify the Human Activities. Human Activity Recoginition and Classification is done using a
<br>VGG19 Model. The CNN model classifies the activities into:
<UL>
  <li>Crawling</li>
  <li>Jumping (includes the possibility of weapons)</li>
  <li>Running/Jogging</li>
  <li>Walking/Marching</li>
  <li>Stone-pelting/Grenade throwing</li>
</UL>
The CNN model architecture uploaded on the repository is designed using <a src="https://www.tensorflow.org/">Tensorflow</a> and is trained on
<br> the dataset: <a src = "https://ieee-dataport.org/documents/diat-%CE%BCradhar-radar-micro-doppler-signature-dataset-human-suspicious-activity-recognition"> DIAT-μ RadHAR (Micro-Doppler Signature Dataset) </a> available at <a src="https://ieee-dataport.org/"> IEEE Dataport </a> 
