```
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

```

## Case Study of the DAPAR Robotics Challenge

- Stability
  - Number and geometry of contact points
  - Centre of gravity
  - Static/dynamic stability
  - Inclination of terrain
- Characteristics of contact
  - Contact point/path size and shape
  - Angle of contact
  - Friction
- Types of environment
  - Structure
  - Medium (air, water etc)

## Wheeled Robots

- It is the most popular locomotion mechanism due to:

  - Good efficiency
  - simple mechanical implementation
  - Easy balance
- Four major wheel classes

  - Standard wheel: 2 DOF
  - Castor Wheel: 2 DOF
  - Swedish/Mecanum Wheel: 3 DOF
  - Ball/spherical Wheel: 3 DOF

### Motor Classification

- DC motors
  - Brushed Motors
  - Brushless motors
  - Servo motors
- AC Motors
  - Induction motors
  - Synchronous motors
  - Servo motors
  - Stepper Motor

### Three fundamental characteristics for locomotion

- Stability
  - Number of wheels and the configuration
- Maneuverability
  - How easily the robot can be manoeuvered
- Controllability
  - How easily the robot can be controlled
  - Generally inverse to maneuverability

---

## Kinematics for Differential Drive Robot

#### Wheel Rotation and Velocity Relationship

![1622593601169.png](./1622593601169.png)

Assuming no Slippage

$V_{wheel}$ = $\omega_{wheel}$*$r_{wheel}$
