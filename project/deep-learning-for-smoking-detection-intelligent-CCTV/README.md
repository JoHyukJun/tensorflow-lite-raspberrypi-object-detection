# Deep Learning for Smoking Detection Intelligent CCTV

### Author: Jo Hyuk Jun


## Overview

최근 금연 구역의 증가하는 추세를 볼 수 있다. 하지만 금연 구역에서 흡연을 하는 경우를 사람이 일일일 모두 찾아 낼 수 없으며 이러한 감시 비용에 큰 사회적 비용을 지출할 수 있다. 현재 Deep Learning 을 이용한 Object Detection 의 성능은 CNN(Convolution Neural Network) 을 통해 상당한 수준의 정확도를 보여준다. 이를 이용하여 라즈베리 파이와 같은 저렴한 비용으로 구현할 수 있는 시스템에서 담배 이미지들을 학습한 딥 러닝 모델을 통해 카메라에 입력받은 영상에서 흡연을할때 사용하는 담배를 검출할 수 있는 지능형 CCTV를 본 프로젝트에서 구현하기로 기획했다.


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
