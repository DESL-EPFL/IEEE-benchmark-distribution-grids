# IEEE-benchmark-distribution-grids
The network data of IEEE benchmark distribution grids
'IEEE_node25.mat', 'IEEE_node69.mat', and 'IEEE_node123.mat' are MAT files that consist of network data, peak demand value at each node, and PV capacities.
Each file has 2 structure arrays:
1. Ginput: Network data 
VV : Base volatge / sqrt(3)
AA : Base power / 3
LineParam : Line parameters
    1st and 2nd column : Sending end (node) and receiving end (node)
    3rd column : resistance (ohm/km)
    4th column : reactance (ohm/km)
    5th column : susceptance (s/km)
    6th column : ampacity (A)
    7th column : line length (km)
    8th column : Type of line: 1 - overhead line, 2 - underground cable
    
2. Linput: Location of demand and its peak values, location of PV panels and their capacities
PVnodes : Nodes with PV panels and the capacities
    1st column : Node with PV panels
    2nd column : PV capacities 
Loadnodes : Nodes with load consumption
PQ : Peak active/reactive demand at each node
    1st column : Node 
    2nd column : Peak active demand (kW)
    3rd column : Peak reactive demand (kVAR)
  
