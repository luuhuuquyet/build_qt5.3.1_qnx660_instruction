## How to build the QT5.3.1 for QNX6.6

### Go to the qt site and download the qt5.3.1 source:
Download: [Qt5.3.1](https://download.qt.io/new_archive/qt/5.3/5.3.1/single/qt-everywhere-opensource-src-5.3.1.zip)

### Get QNX660 SDP from QNX
Or we can get it from some of sharing: [qnx660](https://github.com/unclassified-org/QNX-SDP)
### Do build
```
source /opt/qnx660/qnx660-env.sh 
unzip -a qt-everywhere-opensource-src-5.3.1.zip 
mkdir build 
cd build 
../qt-everywhere-opensource-src-5.3.1/configure -opensource -confirm-license -xplatform  qnx-armle-v7-qcc -release -qpa qnx -prefix <your install directory> 
make 
make install 
```
### GoodLuck
