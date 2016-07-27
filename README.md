

# dcn_simulation_using_mininet
This is the project for the USTC course CS05112, which was finished in 2015 fall semester.

Datacenter Network Simulation using Mininet

Objective:
Simulate the FatTree datacenter network using Mininet and MinEdit.
1.With controller: spamming tree, link failures
2.Without controller: implement FatTree’s routing rules with switch flow rules

Experiment 1 (with controller)
1.The physical topology has loops, you need to first build a logical spamming tree (hint: use the existing)
  Figure out and draw the logical spamming tree topology
2.Make OpenFlow switches to behave like address learning switches 
  Using pingall to testify, examine the flow tables on switches
3.Introduce link failure events with at least three simultaneously failed links
  However, the physical network shouldn’t be partitioned. 
4.Reconstruct the spamming tree and re-populate the flow tables with pingall
  Topology, pingall result, flows table on switches

Experiment 2 (without controller)
1.Do not use any controller
2.In simulation script, insert appropriate flow table entries in OpenFlow switches to make the network behaves like FatTree.
3.Test the routing rules with pingall
4.Prove that the traffic is evenly distributed on FatTree with flow table entry statistics.
