# ros_screencast
ros node which publishes the whole X screen on an Image topic.

## Build
    cd ~/catkin_ws/src
    git clone https://github.com/herr-biber/ros_screencast
    pip install -r ros_screencast/requirements.txt --user
    cd ~/catkin_ws
    catkin_make install
  
## Demo
Run screencaster and image_view (demo)

    roslaunch ros_screencast screencast_view.launch
    
## Parameters 
    rosrun ros_screencast screencast
    
* `_no_alpha`: (bool) Whether to publish bgr8 instead of bgra8 encoding (default true)
* `_rate`: (double) The rate (in hz) at which to publish (default 15.0)
* `_frame_id`: (str) The frame_id to put in Image header (default "screen")
* `_topic`: (str) The topic name to publish screen images on (default "screen")
