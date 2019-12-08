# Deep Learning for Smoking Detection Intelligent CCTV

### Author: Jo Hyuk Jun


## Overview

You can see the recent trend of non-smoking areas. However, people who smoke in non-smoking areas cannot be found every single day, and they can spend a lot of money on monitoring. Current Object Detection performance using Deep Learning shows a significant level of accuracy through CNN(Convolution Natural Network). Through Deep Learning Model that learned smoking images from systems that can be implemented at low cost, such as raspberry pi. The project plans to implement intelligent CCTV that can detect tobacco used to smoke in images entered into the camera.


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
python3 detect_smoking.py \
  --model ${DATA_DIR}/model/detect.tflite \
  --labels ${DATA_DIR}/model/labelmap.txt
```


## Reference
> https://github.com/tensorflow/examples/tree/master/lite/examples/object_detection/raspberry_pi
