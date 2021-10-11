# udm_kajal_jyotika_gb
#Head to the folder src

git clone https://github.com/jyotika02/udm_kajal_jyotika_gb.git

cd ..

catkin build

source devel/setup.bash

roslaunch turtlebot3_gazebo turtlebot3_world.launch

roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml

rosrun udm_kajal_jyotika_gb global_localization.py
