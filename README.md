# Grotifer Satellite Project

Research for the GROTIFER Project (funded by NASA's Heliophysics Technology and Instrument Development for Science program) was conducted at UC Berkeley's Space Sciences Lab. The goal of this research was to develop a cube satellite that could accurately measure three-dimensional electric and magnetic fields, as well as the velocity distribution functions of the charged particles that interact with those fields.

In our work, we were able to demonstrate the three-dimensional controllability of a satellite prototype  under a constant steady-state torque from orthogonal rotating booms on a simulated weightless lab testbed.

<video src="https://github.com/user-attachments/assets/4fb844cc-0ef4-4873-8588-3f9f4d901125" controls></video>

# Code organization

### docs
Contains documentation for the project and a pdf detailing attitude control strategy.

### external
Contains external hardware header files.

### include
Contains all project header files.

### src
Contains all project .cpp files.

# Task Descriptions

### Attitude Control Task
Directs the operation of the attitude control actuators

### Torp Control Task
Directs the operation of the actuators on the rotating booms.

### Task Coordinator
Coordinates the timing and operations of the other tasks.
