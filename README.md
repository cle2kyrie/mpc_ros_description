# mpc_ros_model

## 概述

此存储库支持“mpc_ros”存储库，用于控制各种模型（如差速驱动模型、阿克曼模型、完整驱动模型）。它整合了来自其他公共包的各类模型，因此您可以分别克隆这些参考代码。

## 要求
``` 使用以下命令进行安装：sudo apt-get install ros-melodic-hector-gazebo-plugins ros-melodic-ackermann-steering-controller ros-melodic-rqt-robot-steering ```

## 启动模型

### 差速驱动模型

```ros启动文件 mpc_ros_description/differential_model.launch```

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ef45e537-291a-4fee-80bd-acacb4118c13/Screenshot_from_2021-02-08_13-16-13.png](./assets/diff_model.gif)

阿克曼模型

```ros启动文件 mpc_ros_description 目录下的 ackermann_model.launch 文件```

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ef45e537-291a-4fee-80bd-acacb4118c13/Screenshot_from_2021-02-08_13-16-13.png](./assets/ackermann_model.gif)

### 自行车模型
```roslaunch mpc_ros_description bicycle_model.launch```

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fd751637-0aae-49da-ad90-e07a13ad4369/bicycle.gif](./assets/bicycle_model.gif)

### 洛根尼模型
```roslaunch mpc_ros_description holonomic_model.launch```

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5fddeff9-52f5-4a36-a245-4fdb19538759/Untitled.png](./assets/holonomic_model.gif)



可以根据参数选择相应的模型

```ros启动文件 mpc_ros_description/models.launch```



## 参考文献

- [服务机器人](https://github.com/CzJaewan/servingbot)
- [差速驱动](http://wiki.ros.org/differential_drive)
- [转向驱动控制器](http://wiki.ros.org/steer_drive_controller)
- [转向驱动ROS](http://wiki.ros.org/steer_drive_ros)
- [赫克托Gazebo插件](http://wiki.ros.org/hector_gazebo_plugins)
