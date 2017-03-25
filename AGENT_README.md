Mininet AGENT: A Node That Enables Monitoring The Switch 
========================================================

*This project was done as part of our !*

Agent 1.0

### What is An Agent?

Agent is a subclass node that shares the same network namespace as 
the switch and the controller. Since it is a subclass to the node it
can also connect by link to any other component in the network.

Agents supply the basic infrastructure for creating user defined monitoring 
applications in the network. The first subclass Agent we added is an OpenFlow
based Agent that connects to the OpenFlow switch, called – OpenFlowAgent. 
The first two use-cases that give an example on what an Agent can be used for are:
•	SamplingAgent - samples every N packet that arrives to the switch.
•	SecAgent - samples every packet that arrives to the switch after N seconds.

### How does it work? Ryu maneger application?
* (Choose) Two new topologies: SingleSwitchAndAgentTopo(topo), TwoSwitchAndAgentTopo(topo).

### Features Added to Mininet


* 

### Documentation

ppt
doc?


Shira Levy & Sivan Oddes 
Guided by: Jalil Morany & Itzik Ashkenazi 
