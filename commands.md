# Isaac Sim + ROS 2 Jazzy Commands

## Launch Isaac Sim
```zsh
conda deactivate
source /opt/ros/jazzy/setup.zsh
~/isaac-sim/isaac-sim-standalone-5.1.0-linux-x86_64/isaac-sim.sh
```

## Inside Isaac Sim
1. Window → Extensions → search "ROS2" → Enable
2. Create ActionGraph: Stage → Create → Visual Scripting → Action Graph
3. Add nodes: Isaac Read Lidar Beams, ROS 2 Publish Laser Scan, Isaac Read Simulation Time, On Playback Tick
4. Press Play

## ROS 2 (new terminal)
```zsh
source /opt/ros/jazzy/setup.zsh
ros2 topic list
rviz2
```

## RViz Setup
1. Fixed Frame → `sim_lidar`
2. Add → By Topic → `/scan_lidar` → LaserScan → OK
