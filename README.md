# Traffic Light Simulation and Optimisation using YOLO with OpenCV
Contributors  - Gautam Bhatia , Vatsal Malviya

Technology Used - YOLO(You Only Look Once) and Open CV

Google Drive Link for yolov3.weights - https://drive.google.com/file/d/1zG8eZrdfzzNyOcIiLyIxo5o-pH4643Zx/view?usp=sharing

### How to install prerequisites?
"pip install opencv"

Note : yolo trained model is already added as yolov3.weights

### Why This project?
On average, travellers in Delhi, Mumbai, Bengaluru, and Kolkata spend 1.5 hours more on their daily commutes
than their counterparts in other Asian cities during peak traffic times, according to an April 18 report 
released by The Boston Consulting Group (BCG) and commissioned by Uber.
Even then Indian Roads are not eqipped with any smart technology to reduce the a person time on the signals.
Some European countries have implemented signal time simulation using electromagnetic signal detectors but 
problem with this is that it is a very expensive method also requires alot of maintainence work which is furthur
very expensive 
So we have implemented signal time optimisation using traffic detection which is quite good and very less expensive

### How we have Implemented this?
We have firstly trained the images for object detection using YOLO(you only look once) algorithm and stored the trained data in
the yolov3.weights file , yolov3.cfg for configuration file and coco.names for classes of all the objects which can be detected
and then used Open Cv to detect and count the traffic from the image and due to direct proportion of no of cars and time of signal 
light we have made a y=Mx+c type relation and manually set M as 3 as from general observation a car takes 3 second to cross a signal 
and Then used this Y=MX relation to predict furthur inputs here for X=0 ,Y should be 0 from this c becomes 0 and we get Y=3X.

### Further Development of the project possible?
1) M can be calculated from Linear Regression by collecting the data from cctv footage and labeling them. 
This can furthur increase the accuracy of the time predicted also if more images are taken to train the Yolo model we get more and more correct classification.
2) Connect the CCTV footage of all the cross-sections and give a more beneficial traffic management plans by using Historical data.( Eg. Making Roads One-Way during Rush Hours )
      
 
  
 

