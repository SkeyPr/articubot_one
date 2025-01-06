Differential Drive Robot Simulation

This repository contains the URDF and configuration files for simulating a differential drive robot in ROS 2. The robot is designed with a simple yet robust structure, making it suitable for applications like navigation, mapping, and obstacle avoidance.
Features

    Chassis:
        A lightweight, rectangular base for the robot's body.
        Designed with accurate inertial properties for realistic simulation.

    Differential Drive System:
        Two driven wheels (left and right) controlled via continuous joints.
        Allows the robot to perform precise linear and rotational movements.

    Caster Ball:
        A passive spherical ball mounted at the rear for balance and stability.
        Configured with minimal friction for smooth motion.

    Gazebo Integration:
        Material definitions for realistic visualization in the Gazebo simulator.
        Configured collision properties and friction coefficients for accurate physics.

File Structure

    robot.urdf.xacro:
        Main URDF file that defines the robot's structure and includes the following components:
            Chassis
            Left and Right Wheels
            Caster Ball
            Inertial properties

    inertial_macros.xacro:
        Macros for defining inertial properties of the robot components.

    Sensor Integration:
        Additional URDF files for integrating sensors like lidar and cameras.

Prerequisites

    ROS 2 Humble or later
    Gazebo for simulation

Getting Started

    Clone the repository:

git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

Build the workspace:

colcon build

Launch the simulation:

ros2 launch your_package_name launch_sim.launch.py

Visualize in Rviz:

    rviz2

Future Work

    Adding sensor integration (e.g., lidar, camera) for advanced functionalities.
    Implementing SLAM and navigation algorithms.
    Testing in real-world environments with hardware.

Contributing

Contributions are welcome! Feel free to open issues or submit pull requests for new features or bug fixes.
License

This project is licensed under the MIT License.