# Trajectory Error Estimation
## Introduction
The trajectory error estimation in the SLAM.  
Besides, this project also contains a file showing how to use Sophus package.

## Requirements
### Eigen Package (Version >= 3.0.0)
#### Source
http://eigen.tuxfamily.org/index.php?title=Main_Page

#### Compile and Install
```
cd [path-to-Eigen]
mkdir build
cd build
cmake ..
make 
sudo make install 
```

#### Search Installing Location
```
sudo updatedb
locate eigen3
```

default location "/usr/include/eigen3"


### OpenGL Package (use pangolin)
#### Download
https://github.com/HugoNip/Pangolin

#### Install the dependency for pangolin (mainly the OpenGL)
```
sudo apt-get install libglew-dev
```

### Sophus Package
#### Download
https://github.com/HugoNip/Sophus

#### Compile and Install
```
cd [path-to-pangolin]
mkdir build
cd build
cmake ..
make 
sudo make install 
```

## Compile this Project
```
mkdir build
cd build
cmake ..
make 
```

## Run
```
./trajectoryError
./useSophus
```
## Reference
[Source](https://github.com/HugoNip/slambook2/tree/master/ch4)
