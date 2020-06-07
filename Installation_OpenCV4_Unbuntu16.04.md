### Install dependancies <br/>
`sudo apt-get -y install libopencv-dev build-essential cmake libdc1394-22 libdc1394-22-dev libjpeg-dev libpng12-dev libtiff5-dev libjasper-dev libavcodec-dev libavformat-dev libswscale-dev libxine2-dev libgstreamer0.10-dev libgstreamer-plugins-base0.10-dev libv4l-dev libtbb-dev libqt4-dev libmp3lame-dev libopencore-amrnb-dev libopencore-amrwb-dev libtheora-dev libvorbis-dev libxvidcore-dev x264 v4l-utils` <br/>

### Download and build opencv4 <br/> 
`wget "https://github.com/opencv/opencv/archive/4.0.0.tar.gz" -O opencv.tar.gz` <br/>
`wget "https://github.com/opencv/opencv_contrib/archive/4.0.0.tar.gz" -O opencv_contrib.tar.gz ` <br/>
`tar -zxvf opencv.tar.gz ` <br/>
`tar -zxvf opencv_contrib.tar.gz` <br/>
`cd opencv-4.0.0` <br/>
`mkdir build ` <br/>
`cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/full/path/to/opencv-4.0.0/build -D INSTALL_C_EXAMPLES=ON -D BUILD_EXAMPLES=ON -D OPENCV_EXTRA_MODULES_PATH=/full/path/to/opencv_contrib-4.0.0/modules ../ ` <br/>
`` <br/>
