# rosbag2video

A simple utility to convert ROS `sensor_msgs/Image` messages into a video from
a rosbag. Usage is straightforward:
```
rosbag2video.py bagfile [-e encoding]
```
Here you specify the bag file from which to parse Images, and optionally the
desired encoding for the video. Currently, the default and only supported
option is `.avi`.

The script will automatically find all of the `sensor_msgs/Image` topics in the
bag file and write them out to video files.
