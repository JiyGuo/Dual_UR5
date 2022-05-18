# Dual_UR5

启动前请检查与机器人连接情况
```
ping {robot_ip}
```
启动双臂机器人：
```
cd {your workspace}
catkin_make
source devel/setup.bash
roslaunch uu_robot dual_ur5_bringup.launch
```
启动后会打开rviz可视化工具，如果显示界面与当前机器人构型一致，说明已经成功与机器人建立连接。
在控制机器人前，需要手动打开控制器（出于安全性考虑）：
```
rosrun rqt_controller_manager rqt_controller_manager 
```
然后在把控制器都开启。
