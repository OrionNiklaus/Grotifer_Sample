# Grotifer Satellite Project

Research for the GROTIFER Project (funded by NASA's Heliophysics Technology and Instrument Development for Science program) was conducted at UC Berkeley's Space Sciences Lab. The goal of this research was to develop a cube satellite that could accurately measure three-dimensional electric and magnetic fields, as well as the velocity distribution functions of the charged particles that interact with those fields.

In our work, we were able to demonstrate the three-dimensional controllability of a satellite prototype  under a constant steady-state torque from orthogonal rotating booms on a simulated weightless lab testbed.

<video src="https://github.com/OrionNiklaus/Grotifer_Sample/raw/main/Grotifer_rendering.mov" controls></video>

# Code organization

## docs
Contains documentation for the project and a pdf detailing attitude control strategy.

## external
Contains external hardware header files.

## include
Contains all project header files.

## src
Contains all project .cpp files.

# Task Descriptions

## Attitude Control Task
Directs the operation of the attitude control actuators

## Torp Control Task
Directs the operation of the actuators on the rotating booms.

# Task Coordinator
Coordinates the timing and operations of the other tasks.

Grotifer Satellite Project
At Berkeley’s Space Sciences Lab, we are demonstrating controllability of a satellite under a constant steady-state torque from orthogonal rotating booms. These booms enable 3D sensor measurements in space.

My Contributions

Attitude control, actuator/sensor interfaces, logging system, and core algorithms
Heavy use of Eigen for linear algebra
Key Points

Modular architecture: estimation, control, actuators, sensors, and logging sit behind narrow, well-defined interfaces
Abstract interfaces: real hardware and simulations swap without touching control logic
Real-time logging: lock-free ring buffer with a dedicated logging thread to keep control-loop timing deterministic
Attitude determination math: sun-sensor + inclinometer TRIAD method documented in /docs
