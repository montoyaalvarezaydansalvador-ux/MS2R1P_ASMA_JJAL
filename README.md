# MS2R1P_ASMA_JJAL
PRATIAL_3_MS2R1P_SERIAL_MANIPULATOR_ASMA_JJAL

To run the robot simulation, you must first update the file paths in the code:

In the planned_trajectory file:

Modify the path of the points.csv file on line 19 with your specific location.

Update the output path for trajectory.csv on line 197.

In the dxf_exporter_node_v2 node:

Change the default location of trajectory.dxf on line 35.

Do the same with points.csv on line 170.

It is important that you use absolute paths in all cases, not relative ones.

Once these modifications have been made:

Run ros2 launch p3_asma_jjal_2025 robot_launch_ms2r.launch.py to view the static robot in RViz

Launch the planner node with ros2 run p3_asma_jjal_2025 planned_trajectory to start the robot's movement following the contour of the .stl figure


