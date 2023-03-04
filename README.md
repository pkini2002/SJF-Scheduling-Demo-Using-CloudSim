## Problem Statement

The problem of task scheduling is selecting the best suitable VMs or computing resources with the 
consideration of maximizing resource utilization. Our aim is to reduce the total completion time 
(makespan) and the response time with maximizing the resources utilization. We attempt to manage 
the loads between the virtual machines and use the best algorithm to execute the tasks with taking into 
consideration maximizing the resource utilization and reducing the completion time.



## Software Requirements

- Cloud Sim Version - `3.0.3`
- Operating System - Windows/ Linux/ Mac OS
- Commons Math Version - `3-3.6.1`
- IDE Used - `Eclipse`
- JDK Version - `9`

## Hardware Requirements

- RAM 4 GB or more
- Processor Intel or AMD Processor
- Hard Disk 100GB or more

**Note:**

Make sure to change the JDK version of your Eclipse IDE. The JDK Version used in this project is `JDK-9`. This can be done by right clicking on the project folder and then clicking on Java Compiler -> Check Enable Project Specific settings -> Select JDK Version to 9.


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


