# multirobot_formation
基于ros的多机器人仿真（导航+编队）


详细请参考项目笔记（包含导航、编队原理介绍，详细配置过程）：

1、《如何在Gazebo中实现多机器人仿真》 ： https://www.guyuehome.com/4889

2、《基于ROS的多机器人编队仿真》 ： https://www.guyuehome.com/8907

3、《如何在Rviz中实现多机器人导航仿真》 ： https://www.guyuehome.com/8912

4、《基于ROS的多机器人导航+编队仿真》： https://www.guyuehome.com/8915

### catkin_make命令执行时出现的错误：
```
CMake Error at /opt/ros/melodic/share/catkin/cmake/safe_execute_process.cmake:11 (message):
  execute_process(/usr/local/bin/python2
  "/opt/ros/melodic/share/catkin/cmake/parse_package_xml.py"
  "/opt/ros/melodic/share/catkin/cmake/../package.xml"
  "/home/liousvious/multi_robot_formation/build/catkin/catkin_generated/version/package.cmake")
  returned error code 1
```
### 可以通过 `catkin_make --cmake-args -DPYTHON_EXECUTABLE=/usr/bin/python2`命令进行解决。
