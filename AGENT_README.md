Mininet AGENT: A Node That Enables Monitoring The Switch 
========================================================

*This project was done as part of our B.Sc studies at the Technion – Israel Institute of Technology*

Agent 1.0

### What is An Agent?

Agents is a subclass node that shares the same network namespace as the switch and the controller. Since it is a subclass to the node it
can also connect by link to any other component in the network.

### How does it work? 

Agents supply the basic infrastructure for creating user defined monitoring applications in the network. 

* __The first subclass Agent__ we added is called __OpenFlowAgent__- an OpenFlow based Agent that connects 
  to the OpenFlow switch. 
* __The first two use-cases__ that give an example on what an Agent can be used for are:
  * __SamplingAgent__ - samples every N packet that arrives to the switch.
  * __SecAgent__ - samples every packet that arrives to the switch after N seconds.

* __Added two new topologies__: __SingleSwitchAndAgentTopo__(topo) & __TwoSwitchAndAgentTopo__(topo).

Now if you know how to use mininet the rest is the just the same as using any other component in the network. You'll just need to change the Ryu default module- simple_switch to simple_switch_with_agent_support (file attached in Documentation) and run mininet with the above topologies or creat your own!


### On a personal note

We hope our AGENT will help you and that you will create more use cases that are sutable for you and share them with others so we can expand the AGENT toolbox for all of mininet's community.

If you have any questions feel free to write us: sivanoddes@gmail.com, shiralevi51@gmail.com


### Documentation

* final presentation.pptx
* sampelingAgent.avi
* presentation.avi
* Ryu modules: simple_switch_with_agent_


Shira Levy & Sivan Oddes 

Guided by: Jalil Morany & Itzik Ashkenazi 
