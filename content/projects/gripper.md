---
title: "XYZ Gripper Robot"
date: 2022-10-17T23:57:37-04:00
draft: false
type: page
---
Completed: April 2022

{{< youtube V6Dm7wGGrKQ >}}
{{< youtube -Vy11onMYCo >}}

This was my final year capstone project. The client for this project was a material sciences professor. For his research, his group completes many compressions tests of 3D printed components, so our project revolved around removing tedious parts of his project. There were different aspects of the testing process that we could have focused on, but we decided to make a robot that automates the queueing, loading and removal of test samples.

After following the engineering design process, the final result can be seen in the video above. The XYZ Gripper robot, moves between 12 positions in queueing area, grabs a test sample and then moves it onto the test platform. The gripper has a force sensor so it is able to detect any sample between 25 mm and 75 mm. The robot moves in the x, y direction using a belt and stepper motor and the z direction is driven by a lead screw.

{{< figure src="/projects/gripperdrawing.png" alt="Drawing a gripper hand forces" >}}

I was tasked with designing the gripper system for the project. First, I looked at potential gripper designs that were relevant to the problem. I narrowed it down to a rack and pinion gripper due to form factor and simplicity of the mechanism. From there, I calculated the force required by the fingers to lift a sample and then found the required torque the motor would need to provide. Then a motor was selected based on its stall torque and its ability to have force detection. After the motor, I began to cad the gripper, focusing on assembly. I decided to 3D printer the gripper because it allowed for easy manufacturing of custom geometries for the gears, rack and housing.

This was the largest project I've been a part of and I think the most satisfying part was putting all the components together and seeing the robot work as a whole. There was some minor trouble shooting initially but because of our preperation, the robot was able to mostly work right off the bat. 