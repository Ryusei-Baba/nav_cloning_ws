# nav_cloning_ws
## install
[master](https://github.com/open-rdc/nav_cloning/tree/master)   
[pytorch](https://github.com/open-rdc/nav_cloning/tree/pytorch)   
[git branch](https://qiita.com/sunstripe2011/items/53ae4184d021e927b3f3)   

```
cd ~/nav_cloning_ws/src/nav_cloning/
git clone git@github.com:MoriKen254/timed_roslaunch.git
cd ~/nav_cloning_ws/src/nav_cloning/timed_roslaunch/scripts
chmod +x timed_roslaunch.sh
```
```
https://github.com/masakifujiwara1/real_tsudanuma2-3_sim
```
```
https://github.com/masakifujiwara1/draw_nav_cloning
```
```
vim ~/.bashrc
export ROS_MASTER_URI=http://localhost:11311
export ROS_HOSTNAME=localhost
source /opt/ros/noetic/setup.bash
#source ~/orne_ws/devel/setup.bash
source ~/nav_cloning_ws/devel/setup.bash
export PATH=/usr/local/cuda-11.6/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/cuda-11.6/lib64:$LD_LIBRARY_PATH
export TURTLEBOT3_MODEL=burger
export GAZEBO_MODEL_PATH=/home/ryusei/nav_cloning_ws/src/real_tsudanuma2-3_sim/models:${GAZEBO_MODEL_PATH}
```

history
```
vim ~/.bashrc
source ~/.bashrc
cd ~/nav_cloning_ws/src
git clone git@github.com:MoriKen254/timed_roslaunch.git
cd ~/nav_cloning_ws/src/timed_roslaunch/scrips/
chmod +x timed_roslaunch.sh
roscd nav_cloning
git branch
git checkout pytorch
git branch
cd ~/nav_cloning_ws/
catkin_make
 1951  roscd nav_cloning/launch/
 1952  roslaunch nav_cloning_sim.launch 
 1964  roscd nav_cloning/scripts/
 1968  code nav_cloning_node.py 
 1978  roscd nav_cloning/
 1987  roscd turtlebot3_navigation/param/
 1989  code dwa_local_planner_params_waffle.yaml 
 1991  roscd nav_cloning/scripts/
 1993  code nav_cloning_node.py 
```
```
cd ~/nav_cloning_ws/src/nav_cloning/scrips/
code nav_cloning_with_direction_net.py
165行目　 # x_train = self.transform_color(x_train)
（色を自動で補正してしまうためコメントアウトする）
```
