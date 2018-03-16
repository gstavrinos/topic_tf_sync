# topic_tf_sync
roscore

rosparam set use_sim_time true

rosrun tf static_transform_publisher 0 0 0 0 0 0 1 base_link laser 100

rosrun other_node other_node_executable

rosbag play something.bag --clock
