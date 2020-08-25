git clone https://github.com/cmtrom01/uavflight.git  
cd uavflight/flight  
git clone https://github.com/PX4/Firmware.git --recursive  
rename Firmware to 'px4'  
cd px4  
make px4_sitl gazebo (if px4 has not been built before)  
cd ..  
catkin_make  
source ~/uavflight/flight/px4/Tools/setup_gazebo.bash ~/uavflight/flight/px4 ~/uavflight/flight/px4/build/px4_sitl_default  
source devel/setup.bash  
./launch-offb.sh  

##  To Do  
