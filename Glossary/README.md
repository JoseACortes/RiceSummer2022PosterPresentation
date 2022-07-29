# Introduction  
  
## Ongoing Research
  
### RouteNet  

RouteNet is the model from "RouteNet: Leveraging Graph Neural Networks for network modeling and optimization in SDN"  
A paper last updated July of 2020.  
The model is the starting point of the proposed "UnoNet" Model  
  
https://arxiv.org/abs/1910.01508  
  
### UnoNet: Wireless Digital Twin

UnoNet is the Proposed model, based off RouteNet. Currently the project is lead by Abishek Kumar, with Dr Santiago Segarra as an advisor.  
  
## Importance  
  
### simulators  
   
The specific simulator for witch UnoNet is a "digitally twin" in this project is "Network Simulator 3" or "NS3". NS3 is also used to produce the labels for training.  
  
### Digital Twins
  
"Digital Twins" replace models and methods of simulation or other calculation that is "hard-coded" with machine learning models. This is often done for the sake of speed and efficiency.  
  
### topology
  
topology is the structure of a graph, depicted by circles (nodes) and lines connecting them (edges).  
Information of the topology, like the adjacency matrix of nodes, is included in the models input.  
  
### variables
  
The variables of the model currently include the traffics of connections, a variable of edges.  
  
# Background  
  
## Network Modeling
  
### Graphs  
  
Graphs are data structures made up of a topology of nodes and edges.
  
### nodes  
  
Nodes are used to represent items in a system, often users. In this case it represents individual devices in a network.  
  
### edges  
  
Edges are used to represent relationships between items in a system. In this case it represents the connections between devices.  
  
### devices
  
Devices make up a wired or wireless network, and in this case is any electronic that can send or receive digital signals  
  
### data connections

Data connections include any connection between two devices. Routes are a sequence of data connections with a "delay".  

### Graph Neural Networks (GNN's)

Neural Networks are not structured to take graphs by default. GNN's are Neural Network algorithms that are made specifically to learn the embeddings of a graph.

### Topology

Topology is the structure of a graph, depicted by circles (nodes) and lines connecting them (edges).  
Information of the topology, like the adjacency matrix of nodes, is included in the models input.  

### National Science Foundation Topology (NSFNET)

The topology used to train and evaluate the two algorithms. Made up of 14 nodes and 18 edges, with varied traffic data on each of the edges for each sample. Each sample contains data on 10 paths, and a total of 42 path-edge combinations

### traffics

Data variable related to edges, represents the congestion of data between two nodes, based off bandwidth and active communication.

### links

## Inputs and Metrics

### KPI

Key Performance Indicators are diagnosis metrics of a wired or wireless system, used to determine the performance so that other modules of a network optimizer can make decisions.

### delay

Delay is the time it takes for a message to be fully sent from one node to another.

### Mean Squared Error

Mean Squared Error or MSE is the function used to determine loss. Changing the loss function changes how the model is trained.

# Methods and Algorithms

### wired networks

Wired networks are routed by physical means. The original RouteNet was trained using only wired networks

### wireless topologies

Wireless topologies are an extension of their wired counterparts, with considerations such as interference included in the topology.

# Results

## Algorithm Comparison

### MSE loss

Mean Squared Error or MSE is the function used to determine loss. Changing the loss function changes how the model is trained.

### training dataset

The training dataset is made up of 3,593 samples of traffic data and delay labels  

### validation dataset

The validation dataset is made up of 500 samples of traffic data and delay labels

### test-1 data

The training dataset is made up of 1000 samples of traffic data and delay labels  

### test-2 data

The training dataset is made up of 1000 samples of traffic data and delay labels  

# Conclusion

## Future Works

### different topologies

The next topologies to be added

### degrees

Degrees are similar to data on traffics, but is the information on nodes

### capacities

Capacities are similar to data on traffics, but is the information on paths

### accuracy

Increasing accuracy means augmenting the model in hopes of better training. This is at the forefront of the research and is the mathematical part of the project.

### interference

Interference negatively affects the connections between devices on a network. The mathematical modeling of this is still being worked on.