# Battery-Aware-Modelling-and-Analysis-of-a-Sigfox-based-IoT-Network-using-UPPAAL-SMC

This repository contains the energy models of a sigfox based digital wireless sensor node (DWSN) for UPPAAL SMC tool.

# Authors

Muhammad Naeem, 
Brian Nielsen, 
Kim Guldstrand Larsen, 
Michele Albano

# Overview

These models are developed to estimate and optimise the battery lifetime of a DWSN used in a case study aiming to develop an efficient IoT bases water monitoring system.

# Attached files
•	**Data set:** Real sensor measuresments data of water height obtained from the real sensore nodes.

•	**Battery Model of DWSN:** UPPPAL SMC model for DWSN.

•	**UPPAAL SMC:** UPPAAL SMC version used for this project.


# Features
•	Capable of generating the current consumption behaviour of the Sigfox sensor node. 

•	The module can simulate the overall battery life of the sensor node. 

•	It Can generate a comparison of battery life for different transmission strategies.


# Proposed Strategies For transmission
**Worst-case strategy:** 

**Optimise listening strategy:**

**Wether Driven strategy:**

**Data compression Strategy:**


# Processes in Model
•	**Init:** This automaton is used to initialise all processes.

•	**Sensor:** It reflects the sensor node's behaviour and includes all the node's states.

•	**SensorSDC:** The purpose of this automaton is to model the self-discharge of the battery

•	**TableCtrl:** It is used to schedule all actions (sending, measuring and listening) of the node

•	**Weather1:** It includes a probabilistic model for weather prediction.

•	**TableCtrlweather:** This automaton is used as TableCtrl for weather model.

•	**Data:** It process the real sensor measurement of water height to simulate the data compression strategy. 

•	**CompressCtrl:** This automaton is used as TableCtrl for data compression model.


# Future Work
•	implementation of a complete Sigfox IoT solution including network server
