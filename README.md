# Skeleton Trajectory Repository
Welcome to the repository Project of CARI and Vis4Mechs Laboratory, University of Brescia, Italy !<br>

<p align="center">
  <img height="350" src="http://schoolcommunity.altervista.org/uni/immagini/logo.PNG">
</p>
This is a PR test
This repository is a thesis project and aims at developing a ROS-based framework to identify human keypoints and to make the 3d-reconstruction of them inside a collaborative robotic cell, usefull for human movements tracking.

## Start the skeleton node
The entire framework can be executed in a simplified manner for a user by means of a launcher file, which takes care of calling the various nodes:

```bash
roslaunch skeleton_trajectory skeleton_trajectory.launch
```
## Launch parameters
The following parameter is available:
- **kalmanBase**: it specifies the filter typology.
  * <code>kalmanBase:=True</code> is the default condition and performs filtering with the points managed independently of each other (with assumption of constant acceleration in cartesian space).
  * <code>kalmanBase:=False</code> performed filtering with the model of the limb kinematics of person.

## Requirements
- **pyrealsense2**:
```bash
pip install pyrealsense2
```
- **Upgrade scipy**: nedded for rotations
```bash
pip install --upgrade scipy
```
## Maintainers
- Samuele Sandrini, [SamueleSandrini](https://github.com/SamueleSandrini)
- Manuel Beschi, [ManuelBeschi](https://github.com/ManuelBeschi)
