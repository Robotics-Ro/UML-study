# UML 개요
<div style="text-align: right">건국대학교 일반대학원 전기기계 및 전력전자 석사과정 노태형</div><br>

## 서론
일본에서 배웠던 UML을 가지고 소프트웨어 아키텍처 설계의 중요성을 알리기위해 이번 글을 적어봅니다.

목차
- 서론
- 1. UML 이란
- 2. Usecase Diagram
- 3. 
## i. UML 이란
----------------------
1998년 등장한 UML은, 지금은 기술자로써 습득하지 않으면 안돼는 필수 설계기술이 되었다. 
현재, UML은 2.0으로 메이저 버전업을 한 뒤 2.1이 되어 컴포넌트나 엠베디드 시스템에 대응하고 있다.
또한 UML이 ISO 표준이 됨으로 명실상부한 세계기준의 설계표기가 되었다.

UML이란, Unified Modeling Language(통일모델링언어)의 약잘, 시스템의 분서, 설계 실장등을 원만히 진행하기위해 작성된 [모델]의 표기법을 정의한다.
UML은 오브젝트지향기술의 표준화를 진행하기 위해 OMG(Object Management Group)에서 기준이 책정되었다.

UML은 모델링을 위한 언어다. 모델이란 어떠한 대상을 글이나 그림으로 표현하는 것으로, 시스템 개발에 있어 시스템 그 자체가 대상이 된다.
단, UML은 시스템개발방법론(개발의 수단이나 방법론등)을 포함하지 않는다. 때문에 실제 시스템개발에서는 UML과는 별도로 개발방법론을 준비해야한다.

## ii. Usecase Diagram
### - Realsense SDK를 C++로 사용하기 위해서 무엇을 준비해야하는가? 
-------------
OpenCV for C++
RealSense examples have been designed and tested with OpenCV 3.4
https://docs.opencv.org/3.4/d7/d9f/tutorial_linux_install.html

Required Packages
GCC 4.4.x or later<br>
CMake 2.8.7 or higher<br>
Git<br>
GTK+2.x or higher, including headers (libgtk2.0-dev)<br>
pkg-config<br>
Python 2.6 or later and Numpy 1.5 or later with developer packages (python-dev, python-numpy)<br>
ffmpeg or libav development packages: libavcodec-dev, libavformat-dev, libswscale-dev<br>
[optional] libtbb2 libtbb-dev<br>
[optional] libdc1394 2.x<br>
[optional] libjpeg-dev, libpng-dev, libtiff-dev, libjasper-dev, libdc1394-22-dev<br>
[optional] CUDA Toolkit 6.5 or higher<br>

~~~
[compiler] sudo apt-get install build-essential
[required] sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev
[optional] sudo apt-get install python-dev python-numpy libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev libdc1394-22-dev
~~~

CMake
CMake란 여러 환경(window , linux 등)에 맞는 build process를 작성한 것으로, CMakeLists.txt에 기술된 내용을 바탕으로 각 확경에 맞는 Makefile을 생성해 주는 빌드 프로그램이다.

CMake를 통해 Makefile을 만들게 되면, 추가적인 파일이 추가되지 않는 한 Makefile을 수정하지 않고, 자동으로 생성해준다는 장점이 있지만, 단순히 Makefile을 생성해 주는 것이기 때문에 Make를 추가로 해야한다.

Vcpkg
Vcpkg는 Windows, Linux 및 MacOS에서 C 및 C++ 라이브러리를 관리하는 데 도움을 주는 라이브러리입니다.


## 종장

github Address:[https://github.com/Madness-Ro/project-miraisouzouten-document](https://github.com/Robotics-Ro/OpenCV-C--LiDAR)
![example](./images/QR-code.png)
Special Thanks<br>
ROS 국비교육 LiDAR 헤딩 팀


