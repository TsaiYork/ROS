# ROS

#1. Setup your source list
    
    ~>> sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
    
#2. Install
    
    ~>> sudo apt-get update
    ~>> sudo apt-get install ros-indigo-desktop
    ~>> sudo rosdep init
    ~>> rosdep update
    
#3.Confim
  確認是否環境參數配置都以配置好
    
    ~>> export | grep ROS
    
#4.Build workspace

    ~>> mkdir -p ~/name_ws/src
    ~/name_ws >> catkin_make
    ~/name_ws >> source devel/setup.bash
    
