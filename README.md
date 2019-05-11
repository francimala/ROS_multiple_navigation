# Multiple Turtlebot3 navigation
Hi everyone, this is a universiy project I developed with my colleagues Dario Di Domenico, Daniele Gianfagna and Mauro Martini about multiple robot navigation and simulation across multiple machines.

## Project goals
1. Simulation of multiple robot navigation on a single machine. Spawn two Turtlebot3 on a single map and launch the navigation for both.
2. Creation of a node able to send only the closest robot to a specific goal. Python node that given a generic goal defined in RViz is able to understand which is the closest tb3 to that goal and to send it to that position.
3. Simulation of multiple robot navigation across 3 different PCs.

## Documentation
All the documentation, with guides, some theretical issue, troubleshooting ecc. can be found in the PDF file in the repository.

## How to directly use our catkin workspace
To run our launch files and our node, there are two possibilities:
1. Follow the complete procedure that you can find in the PDF file under the paragraph named: “Complete manual procedure”. 
2. Add manually the entire src folder, perform a catkin_make and start using our node and packages.

This is the explanation of the second method (the fastest):
1. Remove the already existing catkin workspace (or rename it to not lose it):

	$ rm -r ~/catkin_ws

**If you already have projects into the catkin_ws directory please do not remove the catkin_ws, only rename it.**

2. Download from our GitHub page the catkin_ws directory with the source folder only:

https://drive.google.com/open?id=1G6ECFKyCK7Ljf4G8wbdKDaSupjOf6l3s

3. Copy it to the “Home” directory of Ubuntu.
4. Open a new terminal and launch:

	$ source ~/catkin_ws/devel/setup.bash

5. Change the directory:

	$ cd ~/catkin_ws

6. Do a catkin_make:

	$ catkin_make


If the catkin_make didn’t report any trouble, you are ready to use all our packages. You will find all the step inside the PDF file under the paragraph “Running multiple robots with our modified launch files”.

Thank you for the attention.
