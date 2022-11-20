<h1>Bernstein-Vazirani_Algorithm_function</h1>

<p>
This algorithm is one of special quantum algorithms which showed that there can be advantages in using a quantum computer as a computational tool for more complex problems. 

There is a function returning the bitwise product of the input with a hidden string of bits  𝑠 . Its length is  𝑛 .

𝑓(𝑥)=𝑠⋅𝑥(mod2)
 
To find the hidden string, we would need to call the function  𝑓  for  𝑛  times. However, using a quantum computer, we can solve this problem with 100% confidence after only one call to the function . 

  The quantum Bernstein-Vazirani algorithm to find the hidden bit string is very simple:
  <br>
  - Initialize the inputs qubits to the state  |0⟩⊗𝑛 , and output qubit to  |−⟩ .
  - Apply Hadamard gates to the input register
  - Query the oracle
  - Apply Hadamard gates to the input register 
  - Measure
  <br>
For more in detailed information about the Bernstein-Vazirani algorithm, feel free to check out this helpful chapter in the Qiskit textbook: https://learn.qiskit.org/course/ch-algorithms/bernstein-vazirani-algorithm.

In the below, there is an example for the Bernstein Vazirani algorithm to find the hidden bit string "111".
 </p>
