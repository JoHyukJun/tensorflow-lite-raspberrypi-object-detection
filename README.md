<a name="readme-top"></a>


[![Activity][activity-shield]][activity-url]
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection">
    <img src="images/logo.png" alt="Logo" width="360" height="360">
  </a>

  <h3 align="center">tensorflow-lite-raspberrypi-object-detection</h3>

  <p align="center">
    An object detection project
    <br />
    <a href="https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://unluckystrike.com/projects/raspberry-pi-lab">View Project</a>
    ·
    <a href="https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/issues">Report Bug</a>
    ·
    <a href="https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://unluckystrike.com/projects/raspberry-pi-lab)

The following source code located in /original/detect_usbwebcam.py is a program that modified this example: [Link](https://github.com/tensorflow/examples/tree/master/lite/examples/object_detection/raspberry_pi). This is another example for Tensorflow lite with Raspberry Pi using USB webcam based on Pi camera version. In this example, you need to add one more from the settings that you performed on the Pi camera version. That is to install opencv.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With


* [![Tensorflow][Tensorflow]][Tensorflow-url]
* [![OpenCV][OpenCV]][OpenCV-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* download model
  ```sh
  curl -O http://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip
  unzip coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip -d ${DATA_DIR}
  rm coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip
  ```

### Installation

Perform the following procedure to install the required package.

1. Clone the repo
   ```sh
   git clone https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.git
   ```
2. Install opencv
   ```sh
   sudo apt-get install libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev
   sudo apt-get install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
   sudo apt-get install libxvidcore-dev libx264-dev
   sudo apt-get install qt4-dev-tools libatlas-base-dev
   sudo pip3 install opencv-python
   ```

### Run
* example
  ```sh
  python3 detect_usbwebcam.py \
  --model ${DATA_DIR}/detect.tflite \
  --labels ${DATA_DIR}/coco_labels.txt
  ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

_For more examples, please refer to the [Documentation](https://unluckystrike.com/projects/raspberry-pi-lab)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add basic modeling type
- [x] Add opencv param data

See the [open issues](https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/amazing-feature`)
3. Commit your Changes (`git commit -m 'feat: Add some amazing-feature'`)
* commit message
  ```git
  <type>[optional scope]: <description>
  
  [optional body]

  [optional footer(s)]
  ```
* commit type
  ```git
  - feat: a commit of the type feat introduces a new feature to the codebase
  - fix: a commit of the type fix patches a bug in your codebase
  ```
4. Push to the Branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

JO HYUK JUN - hyukzuny@gmail.com

Project Link: [https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection](https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Tensorflow](https://www.tensorflow.org/)
* [OpenCV](https://opencv.org)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.svg?style=for-the-badge
[contributors-url]: https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/graphs/contributors
[activity-shield]: https://img.shields.io/github/commit-activity/m/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.svg?style=for-the-badge
[activity-url]: https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/pulse
[forks-shield]: https://img.shields.io/github/forks/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.svg?style=for-the-badge
[forks-url]: https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/network/members
[stars-shield]: https://img.shields.io/github/stars/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.svg?style=for-the-badge
[stars-url]: https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/stargazers
[issues-shield]: https://img.shields.io/github/issues/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.svg?style=for-the-badge
[issues-url]: https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/issues
[license-shield]: https://img.shields.io/github/license/JoHyukJun/tensorflow-lite-raspberrypi-object-detection.svg?style=for-the-badge
[license-url]: https://github.com/JoHyukJun/tensorflow-lite-raspberrypi-object-detection/blob/master/LICENSE
[product-screenshot]: images/screenshot.png
[Tensorflow]: https://img.shields.io/badge/tensorflow-000000?style=for-the-badge&logo=tensorflow&logoColor=white
[Tensorflow-url]: https://www.tensorflow.org/
[OpenCV]: https://img.shields.io/badge/opencv-000000?style=for-the-badge&logo=opencv&logoColor=white
[OpenCV-url]: https://opencv.org