## Problem Statement

The problem of task scheduling is selecting the best suitable VMs or computing resources with the 
consideration of maximizing resource utilization. Our aim is to reduce the total completion time 
(makespan) and the response time with maximizing the resources utilization. We attempt to manage 
the loads between the virtual machines and use the best algorithm to execute the tasks with taking into 
consideration maximizing the resource utilization and reducing the completion time.

This project aims to implement the improved shortest job first scheduling algorithm in cloud computing. 
The already existing shortest job first (SJF) algorithm doesn’t utilize resources efficiently and has higher 
makespan and lower response time. In a scheduling algorithm, the most important parameters to be 
considered are makespan and response time. Therefore, we have implemented the improved SJF 
algorithm which maximizes the resource usage and efficiency, as well as minimize the completion time 
of the last task (Makespan) and the average response time.

## Steps to run the project

- Open the project in the Eclipse IDE
- Open the examples folder of the project and navigate to `org.cloudbus.cloudsim.examples` and Open the `Simulation.java` file
- Right click on Simulation.java file and then click on Run as 1 Java application. You can then view the creation of datacenter and task scheduling jobs being performed in the console

*Note: If you encounter a launch error 'Main type not found' error then close your project and reopen it and try running the Simulation.java file*
*All other files present in examples folder are demo files representing different tasks and are not a part of our project. Feel free to delete them if you feel the project structure as complex*

> For those creating the project from start the following changes needs to be made in the cloudsim setup code

- Replace the DataCenterBroker.java code with the one used in the project. The default code provided by cloudsim is of FCFS Task Scheduling
- Create a new Java class called `Simulation.java` in examples folder and paste the code from the above respective folder 

## Software Requirements

- Cloud Sim Version - `3.0.3`
- Operating System - Windows/ Linux/ Mac OS
- Commons Math Version - `3-3.6.1`
- IDE Used - `Eclipse`
- JDK Version - `18` (JDK Version 9 or higher would suffice)

## Hardware Requirements

- RAM 4 GB or more
- Processor Intel or AMD Processor
- Hard Disk 100GB or more

**Note:**

Make sure to change the JDK version of your Eclipse IDE. The JDK Version used in this project is `JDK-9`. This can be done by right clicking on the project folder and then clicking on Properties -> Java Compiler -> Check Enable Project Specific settings -> Select JDK Version to 9.


## Some Useful links:

- <a href="https://github.com/Cloudslab/cloudsim/releases/tag/cloudsim-3.0.3">Cloudsim Installation</a>
- <a href="https://archive.apache.org/dist/commons/math/binaries/">Commons-Math</a>


## Installation

**Prerequisites**
- Object oriented aspects of Java programming and its Collections interface.
- Knowledge of cloud computing fundamental concepts.

 ```bash
 git clone https://github.com/pkini2002/SJF-Scheduling-Demo-Using-CloudSim.git
 ```
 
 ```bash
 cd SJF-Scheduling-Demo-Using-CloudSim
 ```
 
**Open the package in any IDE which supports Java and make sure to change the JDK version specified above**

## Implementation
 
 - Initialize the cloudsim package
 ```bash
 Cloudsim.init()
 ```
 
 - Create datacenter
 ```bash
 createDatacenter()
 ```
 
 - Create broker
 ```bash
 createBroker()
 ```
 
 -  Create VMs and cloudlets
 ```bash
createVM()
createCloudlet()
 ```
 
 - Start the simulation
 ```bash
 Cloudsim.startSimulation()
 ```
 
 - Stop the simulation
 ```bash
 Cloudsim.stopSimulation()
 ```
 
 - Print the list of cloudlets
 ```bash
 printCloudletList()
 ```
 
 ## Research Papers
 
 <a href="https://drive.google.com/file/d/1AfgsvYRY4qcDOg4cDuomknws3fipN5mU/view?usp=sharing">Research Paper on Modified SJF Scheduling Algorithm </a>


