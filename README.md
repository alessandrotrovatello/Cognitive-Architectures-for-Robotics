# Cognitive Architecture for Robotics

This repo contains the final project for the COGAR course at the University of Genoa.

## Context Topic 1

In a partially automated industrial context of automobile production, a state-of-the-art humanoid robot, named H-54, is integrated into the assembly line to perform the task of assembling car doors.
Equipped with an anthropomorphic and articulated structure, H-54 is ouEiFed with a wide range of advanced sensors (two cameras, tactile sensors, proprioception sensors, IMU) and actuators, as well as sophisticated computing and control capabilities (specifically, part of the computation is cloud-based, while part is on-premises on the robot).
At the beginning of its shift, H-54 autonomously positions itself at the warehouse to retrieve the components necessary for door assembly.
Utilising its stereoscopic vision sensors and realtime environment mapping, the humanoid robot plans the most efficient route for transporting materials to the assembly line, avoiding obstacles, and ensuring the safety of surrounding operators.
Once on the assembly line, H-54 places the door components on a worktable and uses its advanced manipulation abilities to perform precision assembly operations.
Thanks to its articulated structure and controlled strength, H-54 can handle delicate components with high precision, such as assembling the electric window regulator, applying the right amount of force according to component specifications.
Its force and tactile sensors constantly monitor material interaction, ensuring accurate execution of operations.
During its shift, H-54 communicates and collaborates with human operators on the assembly line.
Thanks to its advanced communication interface, based on gestures and vocal dialogue, H-54 exchanges realtime information with other human operators and receives instructions to optimise workflow and resolve any operational issues.

## We want to focus on the following situation:
1. While H-54 works on the assembly line, it performs a certain sequence of basic actions to assemble door components, such as the electric window regulator.
H-54 must correctly perceive these components, verify that they are the correct components to be assembled, determine their position in the workspace, and manipulate them appropriately, including using tools; for this purpose, H-54 uses a data structure containing the correct sequences of tasks 
to be performed.
2. Occasionally, while H-54 performs these assembly operations, it must interact with a human operator to receive assistance or perform an operation together.
An example is the cooperative transport of the assembled door to a predefined area of the assembly line. H-54 must then decide based on the estimated weight of the door whether to proceed alone or interact with a human operator; the robot must also decide which human operator to approach.

## Problem
Using points 1/ and 2/ as general rules that H-54 must follow, design a cognitive architecture based on a series of software modules capable of ensuring H-54's overall behaviour given these normative rules.
In particular:
- Use UML formalism to describe the cognitive architecture of H-54, identifying reasonable software components.
- Develop the component diagram of the cognitive architecture, highlighting the cloud-based cognitive components and the on-premises ones.
- Selecting a software module from those provided, describe its state machine explicitly specifying states, events, transitions, and any sub-states.
- Describe the activity diagram of the cognitive architecture.
- Highlight the software components that are "adapters."
- Highlight the software components that are "computational."
- Highlight where the "publish-subscribe" communication mode is used.

---

## Result

![Component diagram](images/component_diagram.jpg)

![Activity diagram](images/activity_diagram.jpg)

![Decision Making System state machine](images/component_diagram.jpg)
