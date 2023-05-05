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
*Or if you encounter some errors in files related to Common Math Library such as Math Utils file try to change JDK version to 1.8 build the project you
will encounter an error in ModuleInfo.java file then again change the JDK Version to 9 and build the project. Now you are good to go and run your project without any errors!*
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
 
 ## Output
 
 ```bash
 Starting SJF Simulation...
Initialising...
Starting CloudSim version 3.0
Datacenter_0 is starting...
Broker is starting...
Entities started.
0.0: Broker: Cloud Resource List received with 1 resource(s)
0.0: Broker: Trying to Create VM #0 in Datacenter_0
0.0: Broker: Trying to Create VM #1 in Datacenter_0
0.1: Broker: VM #0 has been created in Datacenter #2, Host #0
0.1: Broker: VM #1 has been created in Datacenter #2, Host #0
1.Cloudler Id:0,Cloudlet Length:10500
2.Cloudler Id:1,Cloudlet Length:17000
3.Cloudler Id:3,Cloudlet Length:20300
4.Cloudler Id:2,Cloudlet Length:23500
5.Cloudler Id:5,Cloudlet Length:23600
6.Cloudler Id:4,Cloudlet Length:26800
7.Cloudler Id:7,Cloudlet Length:26900
8.Cloudler Id:6,Cloudlet Length:30100
9.Cloudler Id:9,Cloudlet Length:30200
10.Cloudler Id:8,Cloudlet Length:33400
11.Cloudler Id:11,Cloudlet Length:33500
12.Cloudler Id:10,Cloudlet Length:36700
13.Cloudler Id:13,Cloudlet Length:36800
14.Cloudler Id:12,Cloudlet Length:40000
15.Cloudler Id:15,Cloudlet Length:40100
16.Cloudler Id:14,Cloudlet Length:43300
17.Cloudler Id:17,Cloudlet Length:43400
18.Cloudler Id:16,Cloudlet Length:46600
19.Cloudler Id:19,Cloudlet Length:46700
20.Cloudler Id:18,Cloudlet Length:49900
21.Cloudler Id:21,Cloudlet Length:50000
22.Cloudler Id:20,Cloudlet Length:53200
23.Cloudler Id:23,Cloudlet Length:53300
24.Cloudler Id:22,Cloudlet Length:56500
25.Cloudler Id:25,Cloudlet Length:56600
26.Cloudler Id:24,Cloudlet Length:59800
27.Cloudler Id:27,Cloudlet Length:59900
28.Cloudler Id:26,Cloudlet Length:63100
29.Cloudler Id:29,Cloudlet Length:63200
30.Cloudler Id:28,Cloudlet Length:66400
31.Cloudler Id:31,Cloudlet Length:66500
32.Cloudler Id:30,Cloudlet Length:69700
33.Cloudler Id:33,Cloudlet Length:69800
34.Cloudler Id:32,Cloudlet Length:73000
35.Cloudler Id:35,Cloudlet Length:73100
36.Cloudler Id:34,Cloudlet Length:76300
37.Cloudler Id:37,Cloudlet Length:76400
38.Cloudler Id:36,Cloudlet Length:79600
39.Cloudler Id:39,Cloudlet Length:79700
40.Cloudler Id:38,Cloudlet Length:82900
41.Cloudler Id:41,Cloudlet Length:83000
42.Cloudler Id:40,Cloudlet Length:86200
43.Cloudler Id:43,Cloudlet Length:86300
44.Cloudler Id:42,Cloudlet Length:89500
45.Cloudler Id:45,Cloudlet Length:89600
46.Cloudler Id:44,Cloudlet Length:92800
47.Cloudler Id:47,Cloudlet Length:92900
48.Cloudler Id:46,Cloudlet Length:96100
49.Cloudler Id:49,Cloudlet Length:96200
50.Cloudler Id:48,Cloudlet Length:99400
51.Cloudler Id:51,Cloudlet Length:99500
52.Cloudler Id:50,Cloudlet Length:102700
53.Cloudler Id:53,Cloudlet Length:102800
54.Cloudler Id:52,Cloudlet Length:106000
55.Cloudler Id:55,Cloudlet Length:106100
56.Cloudler Id:54,Cloudlet Length:109300
57.Cloudler Id:57,Cloudlet Length:109400
58.Cloudler Id:56,Cloudlet Length:112600
59.Cloudler Id:59,Cloudlet Length:112700
60.Cloudler Id:58,Cloudlet Length:115900
0.1: Broker: Sending cloudlet 0 to VM #1
0.1: Broker: Sending cloudlet 1 to VM #0
0.1: Broker: Sending cloudlet 3 to VM #1
0.1: Broker: Sending cloudlet 2 to VM #0
0.1: Broker: Sending cloudlet 5 to VM #1
0.1: Broker: Sending cloudlet 4 to VM #0
0.1: Broker: Sending cloudlet 7 to VM #1
0.1: Broker: Sending cloudlet 6 to VM #0
0.1: Broker: Sending cloudlet 9 to VM #1
0.1: Broker: Sending cloudlet 8 to VM #0
0.1: Broker: Sending cloudlet 11 to VM #1
0.1: Broker: Sending cloudlet 10 to VM #0
0.1: Broker: Sending cloudlet 13 to VM #1
0.1: Broker: Sending cloudlet 12 to VM #0
0.1: Broker: Sending cloudlet 15 to VM #1
0.1: Broker: Sending cloudlet 14 to VM #0
0.1: Broker: Sending cloudlet 17 to VM #1
0.1: Broker: Sending cloudlet 16 to VM #0
0.1: Broker: Sending cloudlet 19 to VM #1
0.1: Broker: Sending cloudlet 18 to VM #0
0.1: Broker: Sending cloudlet 21 to VM #1
0.1: Broker: Sending cloudlet 20 to VM #0
0.1: Broker: Sending cloudlet 23 to VM #1
0.1: Broker: Sending cloudlet 22 to VM #0
0.1: Broker: Sending cloudlet 25 to VM #1
0.1: Broker: Sending cloudlet 24 to VM #0
0.1: Broker: Sending cloudlet 27 to VM #1
0.1: Broker: Sending cloudlet 26 to VM #0
0.1: Broker: Sending cloudlet 29 to VM #1
0.1: Broker: Sending cloudlet 28 to VM #1
0.1: Broker: Sending cloudlet 31 to VM #1
0.1: Broker: Sending cloudlet 30 to VM #1
0.1: Broker: Sending cloudlet 33 to VM #1
0.1: Broker: Sending cloudlet 32 to VM #1
0.1: Broker: Sending cloudlet 35 to VM #1
0.1: Broker: Sending cloudlet 34 to VM #1
0.1: Broker: Sending cloudlet 37 to VM #1
0.1: Broker: Sending cloudlet 36 to VM #1
0.1: Broker: Sending cloudlet 39 to VM #1
0.1: Broker: Sending cloudlet 38 to VM #1
0.1: Broker: Sending cloudlet 41 to VM #1
0.1: Broker: Sending cloudlet 40 to VM #1
0.1: Broker: Sending cloudlet 43 to VM #1
0.1: Broker: Sending cloudlet 42 to VM #1
0.1: Broker: Sending cloudlet 45 to VM #1
0.1: Broker: Sending cloudlet 44 to VM #1
0.1: Broker: Sending cloudlet 47 to VM #1
0.1: Broker: Sending cloudlet 46 to VM #1
0.1: Broker: Sending cloudlet 49 to VM #1
0.1: Broker: Sending cloudlet 48 to VM #1
0.1: Broker: Sending cloudlet 51 to VM #1
0.1: Broker: Sending cloudlet 50 to VM #1
0.1: Broker: Sending cloudlet 53 to VM #1
0.1: Broker: Sending cloudlet 52 to VM #1
0.1: Broker: Sending cloudlet 55 to VM #1
0.1: Broker: Sending cloudlet 54 to VM #1
0.1: Broker: Sending cloudlet 57 to VM #1
0.1: Broker: Sending cloudlet 56 to VM #1
0.1: Broker: Sending cloudlet 59 to VM #1
0.1: Broker: Sending cloudlet 58 to VM #1
1.4125: Broker: Cloudlet 0 received
3.95: Broker: Cloudlet 3 received
6.9: Broker: Cloudlet 5 received
10.2625: Broker: Cloudlet 7 received
14.0375: Broker: Cloudlet 9 received
17.0995: Broker: Cloudlet 1 received
18.224999999999998: Broker: Cloudlet 11 received
22.824999999999996: Broker: Cloudlet 13 received
27.837499999999995: Broker: Cloudlet 15 received
33.262499999999996: Broker: Cloudlet 17 received
39.099999999999994: Broker: Cloudlet 19 received
40.599: Broker: Cloudlet 2 received
45.349999999999994: Broker: Cloudlet 21 received
52.012499999999996: Broker: Cloudlet 23 received
59.0875: Broker: Cloudlet 25 received
66.575: Broker: Cloudlet 27 received
67.399: Broker: Cloudlet 4 received
74.475: Broker: Cloudlet 29 received
82.77499999999999: Broker: Cloudlet 28 received
91.08749999999999: Broker: Cloudlet 31 received
97.49849999999999: Broker: Cloudlet 6 received
99.8: Broker: Cloudlet 30 received
108.52499999999999: Broker: Cloudlet 33 received
117.64999999999999: Broker: Cloudlet 32 received
126.7875: Broker: Cloudlet 35 received
130.89849999999998: Broker: Cloudlet 8 received
136.325: Broker: Cloudlet 34 received
145.875: Broker: Cloudlet 37 received
155.825: Broker: Cloudlet 36 received
165.7875: Broker: Cloudlet 39 received
167.5985: Broker: Cloudlet 10 received
176.15: Broker: Cloudlet 38 received
186.525: Broker: Cloudlet 41 received
197.3: Broker: Cloudlet 40 received
207.598: Broker: Cloudlet 12 received
208.0875: Broker: Cloudlet 43 received
219.275: Broker: Cloudlet 42 received
230.475: Broker: Cloudlet 45 received
242.075: Broker: Cloudlet 44 received
250.898: Broker: Cloudlet 14 received
253.6875: Broker: Cloudlet 47 received
265.7: Broker: Cloudlet 46 received
277.72499999999997: Broker: Cloudlet 49 received
290.15: Broker: Cloudlet 48 received
297.498: Broker: Cloudlet 16 received
302.5875: Broker: Cloudlet 51 received
315.42499999999995: Broker: Cloudlet 50 received
328.275: Broker: Cloudlet 53 received
341.525: Broker: Cloudlet 52 received
347.39799999999997: Broker: Cloudlet 18 received
354.78749999999997: Broker: Cloudlet 55 received
368.45: Broker: Cloudlet 54 received
382.125: Broker: Cloudlet 57 received
396.2: Broker: Cloudlet 56 received
400.598: Broker: Cloudlet 20 received
410.2875: Broker: Cloudlet 59 received
424.77500000000003: Broker: Cloudlet 58 received
457.098: Broker: Cloudlet 22 received
516.898: Broker: Cloudlet 24 received
579.998: Broker: Cloudlet 26 received
579.998: Broker: All Cloudlets executed. Finishing...
579.998: Broker: Destroying VM #0
579.998: Broker: Destroying VM #1
Broker is shutting down...
Simulation: No more future events
CloudInformationService: Notify all CloudSim entities for shutting down.
Datacenter_0 is shutting down...
Broker is shutting down...
Simulation completed.
Simulation completed.

========== OUTPUT ==========
Cloudlet ID    STATUS    Data center ID    VM ID        Time    Start Time    Finish Time    user id    
    0        SUCCESS        2            1            1.31        0.1            1.41    3
    3        SUCCESS        2            1            2.54        1.41            3.95    3
    5        SUCCESS        2            1            2.95        3.95            6.9    3
    7        SUCCESS        2            1            3.36        6.9            10.26    3
    9        SUCCESS        2            1            3.78        10.26            14.04    3
    1        SUCCESS        2            0            17        0.1            17.1    3
    11        SUCCESS        2            1            4.19        14.04            18.22    3
    13        SUCCESS        2            1            4.6        18.22            22.82    3
    15        SUCCESS        2            1            5.01        22.82            27.84    3
    17        SUCCESS        2            1            5.43        27.84            33.26    3
    19        SUCCESS        2            1            5.84        33.26            39.1    3
    2        SUCCESS        2            0            23.5        17.1            40.6    3
    21        SUCCESS        2            1            6.25        39.1            45.35    3
    23        SUCCESS        2            1            6.66        45.35            52.01    3
    25        SUCCESS        2            1            7.08        52.01            59.09    3
    27        SUCCESS        2            1            7.49        59.09            66.58    3
    4        SUCCESS        2            0            26.8        40.6            67.4    3
    29        SUCCESS        2            1            7.9        66.58            74.47    3
    28        SUCCESS        2            1            8.3        74.47            82.77    3
    31        SUCCESS        2            1            8.31        82.77            91.09    3
    6        SUCCESS        2            0            30.1        67.4            97.5    3
    30        SUCCESS        2            1            8.71        91.09            99.8    3
    33        SUCCESS        2            1            8.72        99.8            108.52    3
    32        SUCCESS        2            1            9.12        108.52            117.65    3
    35        SUCCESS        2            1            9.14        117.65            126.79    3
    8        SUCCESS        2            0            33.4        97.5            130.9    3
    34        SUCCESS        2            1            9.54        126.79            136.32    3
    37        SUCCESS        2            1            9.55        136.32            145.88    3
    36        SUCCESS        2            1            9.95        145.88            155.82    3
    39        SUCCESS        2            1            9.96        155.82            165.79    3
    10        SUCCESS        2            0            36.7        130.9            167.6    3
    38        SUCCESS        2            1            10.36        165.79            176.15    3
    41        SUCCESS        2            1            10.38        176.15            186.53    3
    40        SUCCESS        2            1            10.78        186.53            197.3    3
    12        SUCCESS        2            0            40        167.6            207.6    3
    43        SUCCESS        2            1            10.79        197.3            208.09    3
    42        SUCCESS        2            1            11.19        208.09            219.28    3
    45        SUCCESS        2            1            11.2        219.28            230.47    3
    44        SUCCESS        2            1            11.6        230.47            242.07    3
    14        SUCCESS        2            0            43.3        207.6            250.9    3
    47        SUCCESS        2            1            11.61        242.07            253.69    3
    46        SUCCESS        2            1            12.01        253.69            265.7    3
    49        SUCCESS        2            1            12.02        265.7            277.72    3
    48        SUCCESS        2            1            12.43        277.72            290.15    3
    16        SUCCESS        2            0            46.6        250.9            297.5    3
    51        SUCCESS        2            1            12.44        290.15            302.59    3
    50        SUCCESS        2            1            12.84        302.59            315.42    3
    53        SUCCESS        2            1            12.85        315.42            328.27    3
    52        SUCCESS        2            1            13.25        328.27            341.52    3
    18        SUCCESS        2            0            49.9        297.5            347.4    3
    55        SUCCESS        2            1            13.26        341.52            354.79    3
    54        SUCCESS        2            1            13.66        354.79            368.45    3
    57        SUCCESS        2            1            13.68        368.45            382.12    3
    56        SUCCESS        2            1            14.07        382.12            396.2    3
    20        SUCCESS        2            0            53.2        347.4            400.6    3
    59        SUCCESS        2            1            14.09        396.2            410.29    3
    58        SUCCESS        2            1            14.49        410.29            424.78    3
    22        SUCCESS        2            0            56.5        400.6            457.1    3
    24        SUCCESS        2            0            59.8        457.1            516.9    3
    26        SUCCESS        2            0            63.1        516.9            580    3
Average Response Time of VM-1 : 255.64835
Average Response Time of VM-2 : 171.24646
SJF Task scheduling finished!
 ```
 
 **Modified SJF Scheduling**

*For 20 Cloudlets*

```bash
Average Response Time of VM-1 : 55.649128
Average Response Time of VM-2 : 31.630468
```

*For 40 Cloudlets*

```bash
Average Response Time of VM-1 : 141.89896
Average Response Time of VM-2 : 88.260895
```

*For 60 Cloudlets*
```bash
Average Response Time of VM-1 : 255.64835
Average Response Time of VM-2 : 171.24646
```

**SJF Scheduling**

*For 20 Cloudlets*

```bash
Average Response Time of VM-1 : 141.54948
Average Response Time of VM-2 : 20.39375
```

*For 40 Cloudlets*

```bash
Average Response Time of VM-1 : 391.54913
Average Response Time of VM-2 : 53.64375
```

*For 60 Cloudlets*

```bash
Average Response Time of VM-1 : 751.54865
Average Response Time of VM-2 : 100.64375
```

**FCFS Scheduling algorithm**

*For 20 Cloudlets*

```bash
Average Response Time of VM-1 : 156.02 
Average Response Time of VM-2 : 18.59
```

*For 40 Cloudlets*

```bash
Average Response Time of VM-1 : 422.03
Average Response Time of VM-2 : 49.84
```

*For 60 Cloudlets*

```bash
Average Response Time of VM-1 : 798.03
Average Response Time of VM-2 : 94.84
```

## Result and final Conclusion

We implemented a modified SJF algorithm and compared the result with traditional SJF and FCFS algorithms. The results were compared by running the simulation thrice each time varying the number of cloudlets and the average response time for each VMs

