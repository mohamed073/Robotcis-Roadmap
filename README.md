# Autonomous Robots-Roadmap

A structured learning path to master Autonomous Mobile Robots.

-- **Important notes:**
 1. You have to go in order do not skip any section if you are absoulute begineer, unless you are know what you are doing.

 2. it is prefered to work with newer tool versions of Ubuntue 24.04 LTS, ROS2 Jazzey, and Gazebo Harmonic (you will know it later)
 
 3. Some tutorials below use older versions of ROS1/ROS2 and Gazebo Simulators, it is ok just know the concepts and later you will practice these concepts with the newer versions.

 4. It is recommendent to learn all concepts below with **python** rather than C++, due to it is easy to unserstand so it will rest you from overhead of knowing the syntx of C++ (it is harder than Python), but when you level up you have to learn C++ to work on real robot Projects because it is more effecent.
    
 5. As much as possible Do the execrcieses of the content of each link below to get into Active learning mode (more effecent), not just copy & paste code or watch tutorial as a movie (Passive mode), e.g. try to type the code on your own before see it and compare your own result with the tutorials, do not ignore the tasks, try to convert the ROS1 code into ROS2 (your own version) after search. just remember "practice makes perfect".
    
 7.  4. It is preferred to watch the Repository first and try to understand it, then watch the videos to go into active learning instead of passive learning (lazy mind), this method is more affective in learning process.

    
 8. Make LLM (AI) to help you when you stuck with Errors, convert between different syntax versions e.g.(ROS1 vs. ROS2) if needed.
    
--- 

## Overview 
 
 *What you should understand:* The big picture of Autonomous Robotics.
 
- **[Overview](https://youtu.be/ItqZZ5-2INU?si=0hlkULjL5ICjaPwM)**

---

## Theoretical Concepts

*What you should understand:* The theoretical part of each key subfield (perception, SLAM, planning, control), and common career paths.

- **[Theoretical concepts about each branch](https://github.com/MMSAutonomousTeam/Autonomous-Sessions-2024?tab=readme-ov-file)**

---

## Core Tools

*What you should understand:* Hands-on setup of essential robotics software (Linux, Git, VS Code)

- **[Robotics-Tools Repository](https://github.com/arab-meet/1.Robotics-Tools-Workshop)**  

- **[Robotics-Tools Videos](https://youtube.com/playlist?list=PLYJTYbY2Otg4s7oug2IN6hqwNvP2ksHRx&si=Lfpl1tvFnIq3nWNd)**


  **Notes:**
  1. The version of Linux in the previous tutorial is old. You have to install a newer version that supports ROS2 install Ubuntue 24.04 LTS instead.
  2. There is a practice in the repository that installs a version of ROS1 — ignore it, install **ROS2 Jazzey** instead.
  
---

## ROS2

*What you should understand:* Core ROS2 concepts — nodes, topics, services, actions, and basic CLI tools.
- **[ROS2 Materials (Google Drive)](https://drive.google.com/drive/folders/1Qqz8vPmWGsg4g59m4gcet8XcYW8_MMqJ)**  

*What you should understand:* This is a **review + deeper dive** into ROS2.
- **[BME MOGI - ROS Course](https://github.com/MOGI-ROS/Week-1-2-Introduction-to-ROS2)**  

  **Notes:**
  1. The first link (Google Drive) the lecturer use ROS2 Foxy just ignore it and install the newer version of Ubuntu       & ROS2, same as the commands of installing Gazebo simulator also install the newer version not the one listed in      the tutrials.
  2. the second link it works with the **ROS2 Jazzey** (it is totally ok this version what we are targeting), and it contains the same content as the previous link but with extra concepts with different explaination so it is **optional**, but pay attention that second link you will relay on it to understand some tutorials below, you could just understand the phylosofy that the author type/organize the software with it to be familiar with it.
  
---

## URDF & Simulation

 *What you should understand:* What URDF is (XML format for robot description), how to define links, joints, and visual/collision/inertial properties. Also, basics of simulation environments (Gazebo), Transormation (static & dynamic), and RVIZ.
 
- **[URDF & Simulation (Repository)](https://github.com/arab-meet/3.URDF_Simulation_Workshop)**

- **[URDF & Simulation (Videos)](https://youtube.com/playlist?list=PLYJTYbY2Otg4V0mbKHELr0Zl8MIaFYGMb&si=I6fKnpJc7jhCxBBD)**

- **[RVIZ](https://docs.ros.org/en/humble/Tutorials/Intermediate/RViz/RViz-User-Guide/RViz-User-Guide.html
)**
 
 **Notes:**
  1. The commands in the previous 2 links are assocated with ROS1 it probably will not works for ROS2, Do not worry it     is coverd in ROS2 at the below links, or you can take it an excercise and search how to convert the syntax into ROS2 version as kind of practice.
     
  2. The Version of Gazebo used in the videos is an old version, Do not worry it is coverd at the below links just understand the concepts of simulation, or try to apply the concepts with your own new version of Gazebo (preffered one).

  3. The Robot **Transformation** is very important watch it and understand it carefully, but the syntax it Typed with        ROS1 commands (will not work with ROS2) so try to search how to convert the ROS1 commands into ROS2 that is exists        in the Repository link to work with yours. 
      
 
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
