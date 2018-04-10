# Quantum-Automata
Code for an algorithm that efficiently synthesizes quantum automata by using flowcharts which lowers quantum cost. With the help of Professor Marek Perkowski from Portland State University.

Algorithm from research paper called "Direct Synthesis of Reversible (Quantum) Automata from Flowcharts" by Ankit Gupta, Kevin Wang, Maher Hawash, and Marek Perkowski

Worked with professor Perkowski from Summer 2015-Summer 2016

Algorithm includes converting state machines to exor-friendly flowchart form, going through and listing all the paths from state to state, listing various paths as gates, creating equations for each state, adding ancilla bits for generalized toffoli gates to the point where every gate is either a toffoli, feynman, or not gate, creating quantum circuit to synthesize flowchart, and outputting quantum cost during the synthesis.

The code initially creates two nodes for the start and end states. Can create more initial state nodes if there are more than two states.

There are various methods to create input nodes in between the states. Continuity is created by having the input node have true and false nodes which makes it go to another input node or another state node when the current node is either true or false. Reversibility is accounted for by including previous true and previous false nodes which shows the input or state nodes that led to the current node.

There are methods to account for adding intermediate states in between input nodes by using the same logic above.

Used arraylists to list all the various paths that go from state to state. The arraylist consists of the paths broken up into gates and the gates are cateogorized as toffoli or feynman.

The user manually inputs the flowchart by using the methods to insert input nodes and state nodes.

Then the user can call various other methods that will output the list of paths, type of gates, number of inputs, number of outputs, ancilla bits, and quantum cost for such a manually inputted flowchart.
