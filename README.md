# rtui

rtui is ROS Terminal User Interface

## Support

- Python
  - 3.8+
  - Latest Poetry does not support Python 3.6
- ROS1
  - melodic (Need to use python3.8)
  - noetic
- ROS2
  - foxy+

## Install

Via [pipx](https://github.com/pypa/pipx) (Recommended)

```sh-session
$ pipx install git+https://github.com/eduidl/rtui.git

# melodic
$ pipx install --python python3.8 git+https://github.com/eduidl/rtui.git
```

Pip

```sh-session
$ pip3 install --user git+https://github.com/eduidl/rtui.git

# melodic
$ python3.8 -m pip install --user git+https://github.com/eduidl/rtui.git
```

## Demo

![demo](doc/demo.gif)

## Sub commands

- nodes/topics/services/actions
  - get a list of nodes, topics, or etc.
  - get an information about specific node, topic, or etc.
  - mouse operation
    - click link of a node, a topic, or etc.
  - keyboard operation
    - `b/f`: Trace history backward and forward
    - `r`: Once more get list of nodes, topics or etc.
    - `e`: Start or finish topic subscriptions
    - `q`: Terminate app

## Differnce between ROS1 and ROS2

- ROS1
  - does not support action
- ROS2
  - cannot get server node name from service name
    - Why `ros2 service info` command does not exist?
