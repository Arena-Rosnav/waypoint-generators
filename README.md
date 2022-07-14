# waypoint-generators
This repository implements waypoint generators partly proposed in our paper [Connecting DRL with Conventional Global Planners using Waypoint Generators (IROS21)](https://arxiv.org/pdf/2104.03663).


Waypoint generators are utilized to interconnect learning-based local planners with classic global planners from the ROS Navigation Stack.
Given a global path, the waypoint generators will sample subgoals to shorten the planning horizon of the DRL local planner. Currently, the following
waypoint generators are implemented:
* Subsampling: a simple subsampling of a global path using a predefined lookahead distance (e.g. subsample the global path every 2 meters)
* Spatial Horizon: a more flexible waypoint generator, which calculates the waypoints considering the robot's distance and a lookahead distance.
* Heuristic: a generator based on heuristics. It generates waypoints on the global path but changes the positions based on dynamic obstacles

For more information, we refer to our [paper](https://arxiv.org/pdf/2104.03663).

# Usage
TODO
