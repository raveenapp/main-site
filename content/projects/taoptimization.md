---
title: "TA Allocation Optimization Script"
date: 2022-12-15T09:31:25-05:00
draft: false
type: page
---

Completed: November 2022

The Mechanical Engineering department allocates graduate students as teaching assistants for their undergraduate courses. There are over 100 graduate students that could TA around 50 courses, with each course requiring a different number of TAs. Graduate students can have preferences for their courses and instructors have preferences for graduate students. Allocating the graduate students to courses while taking all of this into account would be a cumbersome and manual task. I was tasked with developing an optimization script to allocate the TAs to their courses instead.

I am familiar with optimization problems through school, but applying to this scale was a new challenge for me. First, I met with a professor who has a similar optimization script for a different department. He outlined for me the types of constraints to use to set up the optimization script. The professor is in a different department which has access to an optimization software that the Mechanical Engineering department does not, so I would have to find a different software to use the same structure with. 

I started by looking into Matlab, I know it is a powerful scripting language and it has an optimization toolbox that I could use. First, I read through the documentation and practiced with the examples they had to understand the toolbox. Then, I broke the optimization script down into 3 parts:
1. processing the survey results
2. the optimizaiton script
3. processing the output into meaningful visuals

I started with 2. as it would take the most time. Using the structure I received as a reference, I worked through importing the data, setting up the constraints, and objective variables. A major obstacle I had to deal with was the fact that the optimization toolbox in MatLab doesn't play well with 3D variables. Since the TAs could be allocated into full TA slot or half TA slot, the output variable has a third dimension. I was able to work around the limitation by breaking the 3D dimensional issues into smaller pieces that could be sorted by the toolbox.

Once I had the optimization script working, I worked on part 1. The survey results with the student and instructor preferences had to be processed into a form that could be used by the script, as the survey should stay the same as every year, and the process could be automated. This involved importing the survey data into MatLab, processing them into separate arrays and outputting them into a spreadsheet. 

Finally, part 3 was organizing the results from the optimization script into an output that could be used by the administrators. As the solution to the optimization script is an array of 1s and 0s, that had to be converted into the TA's name and the equivalent course they are in. 

This was an interesting coding project to throw myself into. There are definitely areas that could be improved where I probably used bad habits or inefficient code but that comes with learning a new skill.