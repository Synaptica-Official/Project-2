## Draw the Kinematic Diagram

1. Sketch the robotic arm, showing all joints and links.
2. Assign coordinate frames to each joint according to the DH convention[1].

## Identify the Four DH Parameters

For each joint, determine the following parameters[2]:

1. **θ (theta)**: Angle about the previous z-axis from the old x-axis to the new x-axis.
2. **d**: Offset along the previous z-axis to the common normal.
3. **r (or a)**: Length of the common normal. For revolute joints, this is the radius about the previous z-axis.
4. **α (alpha)**: Angle about the common normal from the old z-axis to the new z-axis.

## Create the DH Parameter Table

Construct a table with the following format[1]:

| Joint | θ | d | r (or a) | α |
|-------|---|---|---------|---|
| 1     |   |   |         |   |
| 2     |   |   |         |   |
| ...   |   |   |         |   |
| n     |   |   |         |   |

## Fill in the Table

For each joint:

1. Determine θ:
   - For revolute joints: Variable angle of rotation
   - For prismatic joints: Usually 0

2. Calculate d:
   - For revolute joints: Fixed offset along the z-axis
   - For prismatic joints: Variable displacement

3. Measure r (or a):
   - Length of the link along the x-axis

4. Determine α:
   - Angle between successive z-axes

## Special Considerations

- For prismatic joints, d is variable and θ is usually 0[3].
- For revolute joints, θ is variable and d is usually fixed[3].
- The number of rows in the DH table should be equal to the number of joints (or degrees of freedom) in the robot[1].



Citations:

[1] https://automaticaddison.com/how-to-find-denavit-hartenberg-parameter-tables/

[2] https://en.wikipedia.org/wiki/Denavit%E2%80%93Hartenberg_parameters

[3] https://www.youtube.com/watch?v=DPO9Se6ZqN0

[4] https://docs.duet3d.com/User_manual/Machine_configuration/Configuring_Robot_DH_parameters

[5] https://blog.robotiq.com/how-to-calculate-a-robots-forward-kinematics-in-5-easy-steps

[6] https://www.universal-robots.com/articles/ur/application-installation/dh-parameters-for-calculations-of-kinematics-and-dynamics/

[7] https://prajankya.me/dh/

[8] https://users.cs.duke.edu/~brd/Teaching/Bio/asmb/current/Papers/chap3-forward-kinematics.pdf
