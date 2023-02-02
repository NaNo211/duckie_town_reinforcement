# duckie_town_reinforcement

lane following using reinforcment 

Paper: [here](https://github.com/NaNo211/duckie_town_reinforcement/blob/main/RL_Paper.pdf)

source code :[here](https://drive.google.com/drive/folders/1409rPzPuNiJfpoZ_mwMKgyFN-McBk_vt?usp=sharing)

documentation: [here](https://github.com/NaNo211/duckie_town_reinforcement/blob/main/documentation.pdf)

## Introduction
We propose the use of Duckietown, an open-source platform for autonomy education and research, as a hardware implementation for our lane-following task in reinforcement learning. Duckietown includes autonomous vehicles called "Duckiebots" that are equipped with powerful onboard computers, such as Raspberry Pi, and a variety of sensors, including cameras and odometry sensors. The Duckiebots are capable of performing complex single- robot and multi-robot behaviors, making them an ideal platform for autonomy education and research.
we start with The most basic task of the Duckiebot is lane following. 
  - This task is implemented using a realistic computer vision pipeline that contains these steps: 
      1. Capture image
      2. Filter noise (Threshold/Masking)
      3. Detect line lanes
      4.lane centroid is calculated, and error is deduced.
      5. input these calculation in reinforcment learning to start learning and take the next best action

## Model
We need to solve this problem by using reinforcement learning.
OpenAI ROS provide a way to build a reinforcment learning algorithm by using ROS to control the agent(i.e car) 
To make the agent train by itself we will build some parts:
  - Gazebo environment 
  - Robot environment
  - Task environment 
  - learning algorithm(i.e. training script)

## Results
