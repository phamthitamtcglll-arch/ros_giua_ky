# ros_giua_ky
Đinh Văn Hào 23020740	Rotation 	Rotation	LiDAR, IMU, ccamera

Cài đặt
chạy trên Ros1
1. # Các gói phần mềm bổ trợ (Dependencies)

   sudo apt update
   sudo apt install ros-$ROS_DISTRO-gazebo-ros-pkgs ros-$ROS_DISTRO-gazebo-ros-control \
   ros-$ROS_DISTRO-joint-state-controller ros-$ROS_DISTRO-effort-controllers \
   ros-$ROS_DISTRO-position-controllers ros-$ROS_DISTRO-joint-trajectory-controller \
   ros-$ROS_DISTRO-robot-state-publisher ros-$ROS_DISTRO-rviz
   
2. # Cài đặt các thư viện ROS Base

   sudo apt update
   Cài đặt bộ điều khiển cho cánh tay và bánh xe
   sudo apt install ros-noetic-gazebo-ros-control ros-noetic-joint-state-controller \
   ros-noetic-effort-controllers ros-noetic-position-controllers \
   ros-noetic-velocity-controllers ros-noetic-joint-trajectory-controller \
   ros-noetic-diff-drive-controller
   Cài đặt các gói hỗ trợ robot state (để xem trong RViz)
   sudo apt install ros-noetic-robot-state-publisher ros-noetic-rviz
  
3. # Tạo workspace và kích hoạt
   
   Tạo thư mục
   mkdir -p ~/catkin_ws/src\
   Di chuyển vào
   cd ~/catkin_ws/src\
   thả file vào đây
   Biên dịch
   cd ~/catkin_ws\
   Kích hoạt môi trường
   source devel/setup.bash\
   
5. # Cài đặt các thư viện Python
   
   sudo apt install ros-noetic-teleop-twist-keyboard
   
6. # Mở gazebao

   roslaunch my_robot gazebo.launch
   
   # Mở Rviz
   
   roslaunch my_robot display.launch
   
7. # Plugin cho Lidar và Camera trong Gazebo
    
   sudo apt install ros-noetic-gazebo-plugins ros-noetic-gazebo-ros
   
   # Thư viện xử lý dữ liệu IMU
   
   sudo apt install ros-noetic-imu-tools ros-noetic-imu-sensor-controller

   
