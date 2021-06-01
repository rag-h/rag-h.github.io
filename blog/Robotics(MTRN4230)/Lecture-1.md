## What is a robot?
- "A machine capable of carrying out a complex series of actions automatically, especially one programmable by a computer." - Oxford English Dictionary 2016
- These definitions change depending on who you ask and the applications.

## Types of Robots
1. Industrial Robots
    - Used a lot in industrial situations
2. Service Robots
    - Medical
    - Household (robot vacuums etc)
    - Entertainment
3. Military Robots
    - Mostly drives the innovation
4. Space Robots

## Degrees of Freedom
- DOF = axis of movement
- To achieve any location and orientation in space we need 6 degrees of freedom.
    - 3 for position
    - 3 for orientation
- Generally:
    - Robot arm provides 3 DOF for position
    - Robot write provides 3 DOF for orientation (roll, pitch and yaw)

## Joint Types
1. Revolute Joints: Something than can pivot at a single axis. Notated using an R
2. Prismatic Joint: A joint that can extend and retract. Notated using P
3. Spherical joints
These three joints are used to make a robotic arm.

### Articulated Robot
- 5-6 DOF 
- Dextrous and versatile
- Flexible
- Duty cycle can vary

### SCARA
- 3-4 DOF
- Rigid in the direction of the tool z-axiz
- very fast, high productivity
- Simple Kinematics
- Cheap, fast
- Very high duty cycle
- Used generally as pick and place robots

### Cartesian
- Simplest config
- Trivial Inverse kinematic solution
- Typically slower
- Can be made very stiff
- Can be designed very large, and therefore can handle very large loads

### Parallel Robots
- Closed loop by definition
- Forward kinematics problem is complicated
    - In the case of most parallel mechanisms, more than one Cartesian solution usually exist for a given set of joint values.
- Inverse Kinematics is relatively straightforward
    - In the case of serial mechanisms there may be many joint space solutions to a desired end-effector location and orientation
    - In the case of most parallel mechanisms there is usually a unique solution.
- Each manipulator arm will basically have some shake. And every series link will add this uncertainty into the robots end effector. Parallel links will increase the stiffness of the robot. It will reduce the shake in the robots end effector, making it very stable. This increases controllability and increases the speed at which it can move.

## Classification based on Motor Control System
- Servo Control Systems
    - Closed loop feedback control
    - Differentiate between the control signal (set point) and a real value (sensed) used to drive arm motions
    - Control variables include position, speed and power
    - Most robots are servo controlled
- Non-servo Control
    - Open loop, no speed control, only end-position
    - Many pneumatic pick-and-place robots

