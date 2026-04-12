# Autonomous Robots-Roadmap

A structured learning path to master Autonomous Robots.

-- **General notes:**
 1. You have to go in order do not skip any section if you are absoulute begineer.
 2. it is prefered to work with newer tool versions of LINUX OS , ROS2 (Jazzey), and Gazebo
 3. Some tutorials uses older versions of ROS2 and Gazebo Simulators 

--- 

## Overview 
 
 *What you should understand:* The big picture of Autonomous Robotics

- **[Overview](https://youtu.be/ItqZZ5-2INU?si=0hlkULjL5ICjaPwM)**

---

## Theoretical Concepts

*What you should understand:* The theoretical part of each key subfield (perception, SLAM, planning, control), and common career paths

- **[Theoretical concepts about each branch](https://github.com/MMSAutonomousTeam/Autonomous-Sessions-2024?tab=readme-ov-file)**

---

## Core Tools

*What you should understand:* Hands-on setup of essential robotics software (Linux, Git, VS Code)

- **[Robotics-Tools-Workshop Repository](https://github.com/arab-meet/1.Robotics-Tools-Workshop)**  

- **[Robotics-Tools Workshop Videos](https://youtube.com/playlist?list=PLYJTYbY2Otg4s7oug2IN6hqwNvP2ksHRx&si=Lfpl1tvFnIq3nWNd)**


  **Notes:**
  1. The version of Linux in the previous tutorial is old. You have to install a newer version that supports ROS2.
  2. Try to do excercise in the Repo as much as possible
  3. There is a practice in the repo that installs a version of ROS1 — ignore it.
  
---

## ROS2

*What you should understand:* Core ROS2 concepts — nodes, topics, services, actions, and basic CLI tools.
- **[ROS2 Materials (Google Drive)](https://drive.google.com/drive/folders/1Qqz8vPmWGsg4g59m4gcet8XcYW8_MMqJ)**  

*What you should understand:* This is a **review + deeper dive** into ROS2.
- **[BME MOGI - ROS Course](https://github.com/MOGI-ROS/Week-1-2-Introduction-to-ROS2)**  

  **Notes:**
  1. The first link (Google Drive) the lecturer use ROS2 Foxy just ignore it and install the newer version of Ubuntu       & ROS2, same as the commands of installing Gazebo simulator also install the newer version not the one listed in      the tutrials 
  
---

## URDF & Simulation

 *What you should understand:* What URDF is (XML format for robot description), how to define links, joints, and visual/collision/inertial properties. Also, basics of simulation environments (Gazebo), Transormation (static & dynamic), and RVIZ.
- **[URDF & Simulation (Repository)](https://github.com/arab-meet/3.URDF_Simulation_Workshop)**

- **[URDF & Simulation (Videos)](https://youtube.com/playlist?list=PLYJTYbY2Otg4V0mbKHELr0Zl8MIaFYGMb&si=I6fKnpJc7jhCxBBD)**

- **[RVIZ](https://docs.ros.org/en/humble/Tutorials/Intermediate/RViz/RViz-User-Guide/RViz-User-Guide.html
)**
 
 **Notes:**
  1. The commands in the previous 2 links are assocated with ROS1 it probably will not works for ROS2,Do not worry it     is coverd in ROS2 at the below links, or you can take it an excercise and search how to convert the syntax into ROS2.
     
  2. The Version of Gazebo used in the videos is an old version, Do not worry it is coverd at the below links just understand the concepts of simulation, or try to apply the concepts with your own new version of Gazebo (preffered one).

  3. The Robot **Transformation** is very important watch it and understand it carefully, but the syntax it Typed with        ROS1 commands (will not with ROS2) so try to seacrch how to convert the ROS1 commands into ROS2 that is exists        in the Repo link to work with your machine
      
  4. It is preferred to watch the Repository first (first link) and try to understand it, then watch the videos to go into active learning instead of passive learning (lazy mind), this method is more affective in learning process.

 ---
 
 ## URDF & Simulation practial

 *What you should understand:* the practical parts of the theoretical part of **URDF & Simulation** (previous header), but based on ROS2.
 
- **[MOGI-Gazebo-basics Version 1](https://github.com/MOGI-ROS/Week-3-4-Gazebo-basics)**  
 
- **[MOGI-Gazebo-basics Version 2](https://github.com/MOGI-ROS/Week-5-6-Gazebo-sensors)**

  **Notes:**  
  1. Sometimes you can not understand all the syntx of python code e.g. **from launch.launch_description_sources import PythonLaunchDescriptionSource** just copy it and Ask LLM (AI) to help  you understand its purpose and how it works, it will be more engging and make your mind enter active learning state.

---

## SLAM Toolbox & Nav2 Stack

*What you should understand:* how to use slam_toolbox package and integrate it  with Nav2-stack with using turtlbot3.
 
- **[slam_toolbox](https://youtu.be/hMTxb8Y2cxI?si=X1sJJ_XSmUzff2I8)**
  
- **[Nav2](https://youtu.be/idQb2pB-h2Q?si=THcSShyZnrZzLLDC)**

**Notes:**  
1. The previous two links using ROS2-Humble with Gazebo Classic (older versions) so if you stuck with commands just pass it to LLM (AI) to modefy terminal commands for your newer ROS2 version e.g. **sudo apt install ros-huumble-nav2-bringup => sudo apt install ros-jazzy-nav2-bringup (just replace the key word of your ros version)**.

---

## Navigation

*What you should understand:* The implementation of slam_toolbox package & Nav2 Stack in a full project * .
 
- **[MOGI-ROS2-Navigation](https://github.com/MOGI-ROS/Week-7-8-ROS2-Navigation)**
 ---
 
 ## ROS Control 
 
- **[Ros2 Control](https://youtu.be/B9SbYjQSBY8?si=M8A3Nql1-Sd0rWYi)**

**Notes:**  
1. it is mostly needed for real robot when we dealing with hardware component
