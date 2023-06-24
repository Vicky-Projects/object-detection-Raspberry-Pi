# TFODRPi Tensorflow Object Detection Walkthrough with Raspberry Pi
The following repository will allow you to leverage Tensorflow Object Detection models that have been converted to TFLite on a Raspberry Pi.
#  Steps
# Step 1:
Walk through the TFOD tutorial up to step 12 to generate TFLite files:https://github.com/Vicky-Projects/object-detection
# Step 2:
Clone the current repository onto your Raspberry Pi:https://github.com/Vicky-Projects/object-detection-Raspberry-Pi
# Step 3:Install the required dependencies onto your Raspberry Pi
pip3 install opencv-python 

sudo apt-get install libcblas-dev

sudo apt-get install libhdf5-dev

sudo apt-get install libhdf5-serial-dev

sudo apt-get install libatlas-base-dev

sudo apt-get install libjasper-dev 

sudo apt-get install libqtgui4 

sudo apt-get install libqt4-testv

echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list

curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -

sudo apt-get update

sudo apt-get install python3-tflite-runtime

# Step 4: 
Copy your detect.tflite model into the same repository and update the labels.txt file to represent your labels.

# Step 5. 
Run real time detections using the detect.py script

python3 detect.py
