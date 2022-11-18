# simulation_models

This code is a simulation of discrete events (SSD) of a close system formed by 10 working machines.
Machines may fail following a normal distribution.
Mean and deviation can be deduced from "E6.fallos.txt" historical file.
There are 4 extra machines which enter the system in case of machine failure.
There are 3 workers for machine repairing.
Time of repair follows an exponential distribution.
Lambda parameter changes linearly over simulation time.
Total simulation time is 1000 h.
    
The problem modelized consists of 2 nodes:

- Functional system - 10 machines working and 4 extra machines
- Repair service - 3 workers 

Posible events that may change the system's state are: 

- Machine failure
- Machine reparation

We are interested in measuring: 

- Quantity of time workers have been working simultaneously
- Proportion of time the system has been fully working
