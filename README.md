# Quantum-Automata
Code for an algorithm that efficiently synthesizes quantum automata by using flowcharts which lowers quantum cost. With the help of Professor Marek Perkowski from Portland State University.

Algorithm from research paper called "Direct Synthesis of Reversible (Quantum) Automata from Flowcharts" by Ankit Gupta, Kevin Wang, Maher Hawash, and Marek Perkowski

Algorithm includes converting state machines to exor-friendly flowchart form, going through and listing all the paths from state to state, listing various paths as gates, creating equations for each state, adding ancilla bits for generalized toffoli gates to the point where every gate is either a toffoli, feynman, or not gate.

There are various methods to create input nodes in between the states and account for digital quantum logic. 

There are methods to account for adding intermediate states in between input nodes by using the same logic above.

The user manually inputs the flowchart by using the methods to insert input nodes and state nodes.
