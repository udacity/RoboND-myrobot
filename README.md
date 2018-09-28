[![Udacity - Robotics NanoDegree Program](https://s3-us-west-1.amazonaws.com/udacity-robotics/Extra+Images/RoboND_flag.png)](https://www.udacity.com/robotics)
# RoboND-myrobot
myrobot project part of RoboND Gazebo Basics lesson

### Directory Structure
```
    .myrobot                           # myrobot project main folder 
    ├── images                         # Code output image                   
    │   ├── output.png
    ├── model                          # Model files of the two-wheeled robot
    │   ├── robot
    │   │   ├── model.config
    │   │   ├── model.sdf
    ├── script                         # Gazebo World plugin C++ script      
    │   ├── hello.cpp
    ├── world                          # Gazebo main World empty scene
    │   ├── myworld
    ├── CMakeLists.txt                 # Link libraries 
    └──                              
```

### Steps to launch the simulation

#### Step 1 Update and upgrade the Workspace image
```sh
$ sudo apt-get update
$ sudo apt-get upgrade -y
```

#### Step 2 Clone the project folder in /home/workspace/
```sh
$ cd /home/workspace/
$ git clone https://github.com/udacity/RoboND-myrobot
```

#### Step 3 Compile the code
```sh
$ cd /home/workspace/RoboND-myrobot/
$ mkdir build
$ cd build/
$ cmake ../
$ make
```

#### Step 4 Add the library path to the Gazebo plugin path  
```sh
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/workspace/RoboND-myrobot/build
```

#### Step 5 Run the Gazebo World file  
```sh
$ cd /home/workspace/RoboND-myrobot/world/
$ gazebo myworld
```

### Output
The welcome message and the Gazebo World should both launch 
![alt text](images/output.png)


    
 
