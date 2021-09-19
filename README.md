# Genetic-Algorithm-to-find-the-best-logic-circuits

In this project, I implemented a genetic algorithm to find a logical circuit that uses the following gates: <br>

1) And, Or, Xor <br>
2) Nand, Nor, Xnor <br>

The corresponding output for a given binary input is stated in a .csv file. <br>
The circuit takes 10 inputs so we have 2<sup>10</sup> = 1024 possible outputs / rows in the csv file. <br>

One innovation that helped to find the circuit is that I defined the fitness function as follows: <br>
max(number of the correct answers from the actual circuit (x) , number of the correct answers from the inverse of the circuits (i.e. 1024 - x)) <br>
The above fitness function helped to first find the inverse of the actual circuit therefore by adding a not gate at the end of the circuit I was able to find the correct logical circuit.

