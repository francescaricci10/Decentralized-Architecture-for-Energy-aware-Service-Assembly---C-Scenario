# Decentralized-Architecture-for-Energy-aware-Service-Assembly---C-Scenario
This repository contains the simulation code that implements a decentralized architecture to manage an energy-aware service assembly. 
We suppose that each node of the network is powered two different energy sources: a "brown" source, which means non-renewable energy source, 
and a "green" source, a renewable energy source. In particular, we suppose that each node owns a 5x5cm solar panel.

The main features of this project are organized as follow:
- the simulation of the green energy production is managed in src/lnu/mida/controller/SolarController.java
- the controller src/lnu/mida/controller/LinkController.java manages the bindings between services at the end of the gossiping procedure.

