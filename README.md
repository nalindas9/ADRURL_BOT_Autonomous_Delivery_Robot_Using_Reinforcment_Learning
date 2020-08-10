# ADRURL_BOT_Autonomous_Delivery_Robot_Using_Reinforcment_Learning
[![License:MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/nalindas9/ADRURL_BOT_Autonomous_Delivery_Robot_Using_Reinforcment_Learning/blob/master/LICENSE)

## Authors
Nalin Das, Achal Vyas

## About
In this project, we train a delivery robot agent to autonomously pick up and dropoff packages in a warehouse. We use Q-Learning, and Deep Q Learning to remove the
redundancy of planning a path every time a pickup or dropoff location changes.
The task for the robot is to pick up packages from different pickup points and deliver them to any
of the drop-off locations depending upon the requirement. 

## Q Learning

### System and Dependencies
 - Python3
 - Numpy
 - matplotlib
 - math
 - ROS Kinetic (Ubuntu 16.04)
 - Gazebo 7.0.0

### How to Run
1. Clone this repo or extract the "enpm690_final_project_Nalin_Achal.zip" file. <br>
2. Navigate to the folder "Code/qlearning" <br>
3. To run the code, from the terminal, run the command `python3 main.py` <br>
4. The training will first take place after which the testing will be executed.

## Deep Q Network

## System and Dependencies
 - Python3
 - Numpy
 - matplotlib
 - math
 - Tensorflow-cpu
 - Keras
 - ROS Kinetic (Ubuntu 16.04)
 - Gazebo 7.0.0
 
## How to Run
1. Clone this repo or extract the "enpm690_final_project_Nalin_Achal.zip" file. <br>
2. Navigate to the folder "Code/dqn" <br>
3. Before running you need to specify the path to the qlearning folder as the dqn environment uses classes and functions from the qlearning scripts. Specify the path in `sys.path.insert(path to qlearning folder)` at the start. Do this for both `dqn_env.py` and `main.py`<br>
4. To run the code, from the terminal, run the command `python3 main.py` <br>
5. The training will first take place. Once you exit or training end, the training weights will be saved in the same folder.
6. To test, execute the the command `python3 main.py` again, this time it will load the weights and run the testing algorithm.


