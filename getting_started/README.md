1. Get running Ubuntu.  An easy way is to use VirtualBox from [Oracle](https://www.virtualbox.org/wiki/Downloads).  You will also need an ISO file from [Ubuntu](https://www.ubuntu.com/download/desktop)

2. Do some updating and download some required packages

```
sudo apt-get upgrade
sudo apt-get update
sudo apt-get install build-essential
sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev
sudo apt-get install python-dev python-numpy libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev libdc1394-22-dev
```

3. [Download and install](http://docs.opencv.org/2.4/doc/tutorials/introduction/linux_install/linux_install.html) OpenCV

```
cd ~
git clone https://github.com/opencv/opencv.git
cd opencv
mkdir release
cd release
cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..
make
sudo make install
```

4. Install SciPy Stack for analysis
```
sudo apt-get install python-numpy python-scipy python-matplotlib ipython ipython-notebook python-pandas python-sympy python-nose
```
