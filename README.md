# tensorflow-lite-raspberrypi-object-detection

### Author: Jo Hyuk Jun


## Overview

The following source code located in /orginal/detect_usbwebcam.py is a program that modified this example: [Link](https://github.com/tensorflow/examples/tree/master/lite/examples/object_detection/raspberry_pi). This is another example for Tensorflow lite with Raspberry Pi using USB webcam based on Pi camera version. In this example, you need to add one more from the settings that you performed on the Pi camera version. That is to install opencv.



## Download model

```bash
curl -O http://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip
unzip coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip -d ${DATA_DIR}
rm coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip

```

## Install opencv

```bash
sudo apt-get install libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev
sudo apt-get install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
sudo apt-get install libxvidcore-dev libx264-dev
sudo apt-get install qt4-dev-tools libatlas-base-dev
sudo pip3 install opencv-python
```

If you have successfully installed opencv, you can now run this example.


## Run the example


```bash
python3 detect_usbwebcam.py \
  --model ${DATA_DIR}/detect.tflite \
  --labels ${DATA_DIR}/coco_labels.txt
```


## Reference
> https://github.com/tensorflow/examples/tree/master/lite/examples/object_detection/raspberry_pi