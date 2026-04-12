# Autonomous Robots Roadmap

A structured learning path to master Autonomous Mobile Robots.

## Learning Guidelines

1. You must go in order. Do not skip any section if you are an absolute beginner — only skip if you already know what you are doing.

2. It is preferred to work with newer tool versions: **Ubuntu 24.04 LTS**, **ROS2 Jazzy**, and **Gazebo Harmonic** (you will learn about them later).

3. Some tutorials below use older versions of ROS1/ROS2 and Gazebo simulators. That is okay — just understand the concepts. Later, you will practice these concepts with the newer versions.

4. It is recommended to learn all concepts below with **Python** rather than C++, because Python is easier to understand. This will save you from the overhead of learning C++ syntax (which is harder than Python). However, when you level up, you should learn C++ to work on real robot projects, since C++ is more efficient.

5. As much as possible, do the exercises for the content of each link below. This puts you in **active learning mode** (more effective), not just copy-pasting code or watching tutorials like a movie (passive mode). For example:
   - Try to type the code on your own before looking at the solution.
   - Compare your result with the tutorial.
   - Do not ignore the tasks.
   - Try to convert ROS1 code into ROS2 (your own version) after searching.
   
   > Just remember: **practice makes perfect**.

6. It is preferred to first read the repository and try to understand it, then watch the videos. This leads to active learning instead of passive learning (lazy mind). This method is more effective in the learning process.

7. When you explore the tutorials below, you will find that each has its own resources. So do not be a perfectionist and do not go deeper into too many details at once — that will confuse you and overwhelm you rather than teach you. You will learn everything over time when you get your hands dirty with code, not when you explore everything at once. Just be satisfied with the content below. Once you know these basics, you will be able to learn advanced topics based on what you need.

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
1. The version of Linux in the previous tutorial is old. You have to install a newer version that supports ROS2: install **Ubuntu 24.04 LTS** instead.
2. There is a practice in the repository that installs a version of ROS1 — ignore it. Install **ROS2 Jazzy** instead.

---

## ROS2

*What you should understand:* Core ROS2 concepts — nodes, topics, services, actions, and basic CLI tools.

- **[ROS2 Materials (Google Drive)](https://drive.google.com/drive/folders/1Qqz8vPmWGsg4g59m4gcet8XcYW8_MMqJ)**

*What you should understand:* This is a **review + deeper dive** into ROS2.

- **[BME MOGI - ROS Course](https://github.com/MOGI-ROS/Week-1-2-Introduction-to-ROS2)**

**Notes:**
1. The first link (Google Drive) uses ROS2 Foxy — just ignore that and install the newer version of Ubuntu & ROS2. Same for the Gazebo simulator commands: install the newer version, not the one listed in the tutorials.
2. The second link works with **ROS2 Jazzy** (this is the version we are targeting), and it contains the same content as the previous link but with extra concepts and a different explanation, so it is **optional**. Pay attention to the second link because you will rely on it to understand some tutorials below. You could just understand the philosophy of how the author types/organizes the software to become familiar with it.

---

## URDF & Simulation

*What you should understand:* What URDF is (XML format for robot description), how to define links, joints, and visual/collision/inertial properties. Also, basics of simulation environments (Gazebo), transformation (static & dynamic), and RViz.

- **[URDF & Simulation (Repository)](https://github.com/arab-meet/3.URDF_Simulation_Workshop)**
- **[URDF & Simulation (Videos)](https://youtube.com/playlist?list=PLYJTYbY2Otg4V0mbKHELr0Zl8MIaFYGMb&si=I6fKnpJc7jhCxBBD)**
- **[RViz](https://docs.ros.org/en/humble/Tutorials/Intermediate/RViz/RViz-User-Guide/RViz-User-Guide.html)**

**Notes:**
1. The commands in the previous two links are associated with ROS1 and will probably not work for ROS2. Do not worry — this is covered in ROS2 in the links below, or you can take it as an exercise and search how to convert the syntax into ROS2 version as a kind of practice.
2. The version of Gazebo used in the videos is old. Do not worry — it is covered in the links below. Just understand the concepts of simulation, or try to apply the concepts with your own new version of Gazebo (the preferred one).
3. Robot **transformation** is very important — watch it and understand it carefully. The syntax is typed with ROS1 commands (will not work with ROS2), so try to search how to convert the ROS1 commands into ROS2 that exist in the repository link to work with yours.

---

## URDF & Simulation Practical

*What you should understand:* The practical parts of the theoretical part of **URDF & Simulation** (previous section), but based on ROS2.

- **[MOGI-Gazebo-basics Version 1](https://github.com/MOGI-ROS/Week-3-4-Gazebo-basics)**
- **[MOGI-Gazebo-basics Version 2](https://github.com/MOGI-ROS/Week-5-6-Gazebo-sensors)**

**Notes:**
1. Sometimes you may not understand all the syntax of Python code (e.g., `from launch.launch_description_sources import PythonLaunchDescriptionSource`). Just copy it and ask an LLM (AI) to help you understand its purpose and how it works. This will be more engaging and put your mind into an active learning state.

---

## SLAM Toolbox & Nav2 Stack

*What you should understand:* How to use the `slam_toolbox` package and integrate it with the Nav2 stack using TurtleBot3.

- **[slam_toolbox](https://youtu.be/hMTxb8Y2cxI?si=X1sJJ_XSmUzff2I8)**
- **[Nav2](https://youtu.be/idQb2pB-h2Q?si=THcSShyZnrZzLLDC)**

**Notes:**
1. The previous two links use ROS2 Humble with Gazebo Classic (older versions). If you get stuck with commands, just pass them to an LLM (AI) to modify the terminal commands for your newer ROS2 version. Example: `sudo apt install ros-humble-nav2-bringup` → `sudo apt install ros-jazzy-nav2-bringup` (just replace the keyword with your ROS version).

---

## Navigation

*What you should understand:* The implementation of the `slam_toolbox` package & Nav2 Stack in a full project.

- **[MOGI-ROS2-Navigation](https://github.com/MOGI-ROS/Week-7-8-ROS2-Navigation)**

---

## ROS Control

*What you should understand:* ROS2 Control framework for managing robot hardware.

- **[Ros2 Control](https://youtu.be/B9SbYjQSBY8?si=M8A3Nql1-Sd0rWYi)**

**Notes:**
1. This is mostly needed for real robots when dealing with hardware components.

---

> **The rest of this roadmap will focus more on the science of robotics itself, not the software tools.**
