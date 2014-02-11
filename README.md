# Rapidly-exploring Random Trees

A Rapidly-exploring Random Tree is an algorithm used for robot path planning.

This is a Python implementation that uses the Numpy, Matplotlib and Scipy libraries.

The code is implemented on the file *'rrt.py'*. The seventh line of that file is a PNG image representing the map in which the robot has to plan it's route. Images must be black and white, white for free spaces and black for obstacles. Three image files are given as an example.

Once executed the code, you have to clic on the image to select a starting point for the robot, and once again to select a goal point. The algorithm will start generating random points in the image and connecting those points to the nearest point, generating a tree of points.

The most important variables are defined in lines 8-11, these are:

* MIN_NUM_VERT: Corresponds to the minimum number of vertex for the resulting tree, the algorithm will not try to connect to the goal until this number of vertex is reached.
* MAX_NUM_VERT: If the tree has this number of vertex, then the algorithm stops and no path will have been found from the start to the goal points.
* STEP_DISTANCE: Maximum distance between two points.
* SEED: Seed for the random generator.
