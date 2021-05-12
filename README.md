# Decentralized-Architecture-for-Energy-aware-Service-Assembly---C-Scenario
This repository contains the simulation code that implements a decentralized architecture to manage an energy-aware service assembly. 
This project extends the project predented in https://github.com/mi-da/Energy-Aware-Service-Assembly-Journal.

We suppose that each node of the network is powered two different energy sources: a "brown" source, which means non-renewable energy source, 
and a "green" source, a renewable energy source. In particular, we suppose that each node owns a 5x5cm solar panel.


## **Instructions**

- Download the Java Project "Decentralized-Architecture-for-Energy-aware-Service-Assembly---C-Scenario" and import it in your IDE as a Java project
- Link the provided libraries in "ext-lib" to the project
- Input the program argument "configs/mida-assembly-config.txt" (i.e., the configuration file of PeerSim)
- The main class to run the experiments is "peersim.Simulator"


## **Configuration Parameters**

The file configs/mida-assembly-config.txt contains the configuration parameters for the simulation. The main parameters are:

NETWORK_SIZE: The number of nodes in the network

SERVICES_PER_NODE: The number of services hosted by each node

TYPES: Number of types of services

STRATEGY: The selection criteria that the nodes adopt. We implemented multiple strategies:
  1) random
  2) green learning
  3) local energy
  4) fair energy
  5) max balance
  6) max green production


## **New Features**

The main features of this project are organized as follow:
- the simulation of the green energy production is managed in src/lnu/mida/controller/SolarController.java
- the controller src/lnu/mida/controller/LinkController.java manages the bindings between services at the end of the gossiping procedure.

