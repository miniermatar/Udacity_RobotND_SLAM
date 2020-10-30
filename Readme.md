This project is part of the Udacity's Robotic Software Engineer nanodegree program. The objective of the project is to implement SLAM (Simultaneous Localization And Mapping).

## Project setup

1. Create a package called: jm_robot
2. Copy the content of this repository and build the project using catkin_make and source the enviroment
3. To correctly display all the gazebo model in the world, copy the content of the gazebo_model folder to ~/.gazebo/models. Those model were obained from http://data.nvision2.eecs.yorku.ca/3DGEMS/ and are part of the following publcation. A.Rasouli, J.K. Tsotsos. "The Effect of Color Space Selection on Detectability and Discriminability of Colored Objects." arXiv preprint arXiv:1702.05421 (2017). 
4. To run the mapping process, open 3 terminals and launch the following files (using roslaunch)
	roslaunch jm_robot world.launch
	roslaunch jm_robot mapping.launch
	roslaunch jm_robot teleop.launch
5. To run localization process, copy the my_robot/rtabmap.db to the ros default folder: ~/.ros/, open 3 terminals and launch the following files:
	roslaunch jm_robot world.launch
	roslaunch jm_robot localization.launch
	roslaunch jm_robot teleop.launch
