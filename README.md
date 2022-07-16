**Gazebo_blaster**  
This repo is to simulate blaster in gazebo env.  
Due to large mesh files for github upload, the meshes can be download from onedrive [here](https://sutdapac-my.sharepoint.com/:f:/g/personal/shawndy_lee_mymail_sutd_edu_sg/EsQyjp9jQqNPop94Q5KunKcBZ7gmdm3C5dswb5PkM2I1QQ?e=kgyn6l).  
***download the meshes(.stl & .dae) into a meshes folder in ~/meshes***  
  
  
Pre-requisite:
1) make sure you have PX4-Autopilot or Firmware pre-installed onto your system.  
2) already set up your roslaunch px4 posix.launch or px4.launch   
  
To use:  
1) clone this repository onto any directory on your local drive.  
2) terminal 1: $`cd <your-clone-path>/gazebo_blaster/`  
3) terminal 1: $`cp -r ~/meshes/ <your-clone-path>/gazebo-blaster/`
4) open another terminal (2) or tab, $`cd <your-path-to-PX4-Autopilot-or-Firmware>/Tools/sitl_gazebo/models/iris && mv model.config model_iris.config` (this should rename your file and you can close this terminal)  
5) terminal 1: $`cp blaster.sdf model.config <your-path-to-PX4-Autopilot-or-Firmware>/Tools/sitl_gazebo/models/iris`  
6) terminal 1: $ `roslaunch px4 posix.launch or px4.launch` and you should see blaster loaded into gazebo env.  
7) (*Optional*) to insert new plugins into blaster, add into blaster.sdf  
8) Fly  
