6DOF Robot Arm

An open, 3D-printable 6-axis robot arm built from parts most people can get or make themselves: standard NEMA stepper motors, off-the-shelf bearings and 3D printed structure.

Status: work in progress (CAD not finished, first joint being fabricated)
Target: working demonstration by May 2027


ABOUT THE PROJECT

This is my yearly school project at AKG Hungary (www.akg.hu). The goal is to design and build a 6DOF robot arm, including the mechanics, the electronics and the control software.

The main idea is accessibility. Instead of expensive custom actuators or hard-to-find parts, the arm uses common NEMA stepper motors and as many 3D printed parts as possible, so that other makers can reproduce it.

The project is also an application to the Bambu Lab "Let's Make It Fund".


SPECIFICATIONS (TARGET)

Degrees of freedom: 6
Reach: approx. 50-85 cm (aiming for the higher end)
Payload: approx. 300 g (theoretical)
Actuators: NEMA 17 and NEMA 23 stepper motors
Controller: Raspberry Pi 4 B
Motor drivers: TMC5160 breakout boards (to be confirmed)
Structure: mostly 3D printed, with a few aluminium parts


BILL OF MATERIALS (PRELIMINARY)

Motors
- 3x NEMA 17, 20 mm
- 2x NEMA 17, 42 mm
- 1x NEMA 23, 82 mm
(estimated cost: ~90 USD)

Mechanical
- Ball bearings (estimated cost: under 150 USD)
- Aluminium stock for structural parts
- Filament (a filament dryer is planned for some materials)

Electronics
- Raspberry Pi 4 B (chosen for its I/O pins and computing power for kinematics and a possible ML model)
- TMC5160 stepper drivers
- Power supply (still to be decided)
- Custom PCB designed in KiCad


TOOLS AND FABRICATION

- 3D printing: Bambu Lab A1 (plus an enclosed Prusa printer)
- CNC: Makera Air
- Laser cutter for thin wood and quick parts
- PCB design: KiCad
- Control development: MATLAB and Simulink
- Additional tools via the school lab and a Hungarian partner company


ROADMAP

1. Finish the main hardware design
2. Build and test the first joint
3. Design and build the remaining joints one by one (max. ~10 school days per joint)
4. Design the PCB in KiCad
5. Write the control software
6. Integrate, test and tune the full arm
7. Working demo by May
8. Optional extras and improvements after the core arm works


CONTROL SOFTWARE

The control approach is still being decided:

- Inverse kinematics using matrix methods (a semi-working prototype already exists in Excel)
- Possibly a machine learning model, if the math and results justify it

Development and simulation will happen in MATLAB and Simulink.



REPOSITORY CONTENTS (PLANNED)

cad - CAD models and STL files

electronics - KiCad schematics and PCB files

firmware - Microcontroller and Raspberry Pi code

software - Kinematics and control code, MATLAB/Simulink models

docs - Build notes, images and renders
