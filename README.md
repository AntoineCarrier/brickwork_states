# brickwork_states
Code demonstration of important parts and gates of the brickwork states as explained in 
Broadbent, Anne, Joseph Fitzsimons, and Elham Kashefi. 2009. 
“Universal Blind Quantum Computation.” 2009 50th Annual IEEE Symposium on Foundations of Computer Science, October, 517–26. https://doi.org/10.1109/FOCS.2009.36.
\\
This repository contains code showing the workings of parts of the brickwork state "unit cell" and code showing how to build a universal gate set using brickwork states.
In the brickwork state "unit cell" used in this code, qubits are indexed from 0 to 4 on the upper row and from 5 to 9 on the lower layer.
Since there is a known post-measurement correction associated to both possibilities at each measurement, we simulate measurement by projecting onto one of the possibilities
and applying the correction. 
For the three non-trivial gates in the universal gates generating set, we verify the result by applying the inverse of the operation on the final state and checking that 
the result is the initial state of qubits 0 and 5 but transferred on qubits 4 and 9. 