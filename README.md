ROS
===
# 学习ROS（1）

标签（空格分隔）： ROS 学习

---

 1. ROS（Robot Operating System）机器人操作系统，发布是按照字母顺序排列的，其中Fuerte和Groovy相差较大，目前最新版是Indigo,官网地址[ROS官网][1]
 2. 建立工作空间
 http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment
 3. 关于一些package的安装命令
 第一种
---
    $cd ~/ros_workspace
    $git clone git://repository/package_name
    $cd package_name
    $rosmake

 更新

    $roscd package_name
    $git pull
    $rosmake --pre-clean

第二种

    $cd ~/ros_workspace
    $svn checkout http://repository/svn/package_name
    $cd package_name
    $rosmake

更新

    $roscd package_name
    $svn update
    $rosmake --pre-clean

第三种

    $cd ~/ros_workspace
    $hg clone http://repository/package_name
    $cd package_name
    $rosmake

更新

    $roscd package_name
    $hg update
    $rosmake --pre-clean

  [1]: http://www.ros.org/
