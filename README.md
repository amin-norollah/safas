# SAFAS(Secure And FAst hardware Scheduler)

![alt text](https://github.com/amin-norollah/safas/blob/main/Logo-SAFAS.png)

Welcome to the SAFAS, Secure and Fast FPGA-based Hardware Scheduler for Accelerating Task Scheduling in Multi-core Systems.


Description
------------
Hardware scheduler is the concept of separating task scheduling unit from the Operating System(OS) and leaving it to a specific hardware unit for real-time connected embedded systems. Due to the direct access of the hardware scheduler to the processing units and the possibility of parallel control on each unit, the hardware scheduler is expected to increase efficiency and be able to better manage hardware resources than OS in multi-core systems.

In this project, the main goal was to develop hardware to schedule tasks taking into account security issues. Today's embedded systems have the ability to communicate over the internet to realize the IoT technology, they have become very vulnerable to security breaches. The SAFAS suitable for scheduling the high-security, safety critical and their replicas tasks to meet their deadline and can be safe from schedule-base attacks.

This project has been developed with Verilag hardware description language and in its design, an attempt has been made to use the minimum required hardware. The code in this repository has been simplified as much as possible and has been made available to everyone for research purposes.


Structure
------------
The main structure of SAFAS is as follows:

1. The operating system that is responsible for checking the accuracy of the information of each task immediately and sending it to the hardware scheduler.
2. The main queue that has the task of receiving the maximum number of characteristics of real-time tasks.
3. Main hardware scheduler that is responsible for receiving tasks and dispatching them to processing cores.
4. Network on the chip that is responsible for executing tasks (this part is outside the scope of the project).

![alt text](https://github.com/amin-norollah/safas/blob/main/MainArchitecture.jpg)

How to Use
------------
The project consists of two parts:

1. Verilog code that requires software such as xilinx vivado for synthesis and simulation.
2. c++ code that requires the c++ compiler or visual studio software for compiling c++ code that produces a sequence of real-time task characteristics To be able to test the hardware schedule.

