# Quantum Computer Operations

Welcome to the Quantum Computer Operations repository! This collection of code snippets demonstrates the implementation of basic quantum gate operations, including the Hadamard (H) gate and the NOT gate (also known as the X gate).

## Hadamard (H) Gate

The Hadamard gate is a fundamental quantum gate that creates superposition by transforming the basis states |0⟩ and |1⟩ into an equal superposition of both states. The matrix representation of the Hadamard gate is:

H = 1/√2 * [[1, 1], [1, -1]]


### Implementation

The following Python code snippet illustrates how to perform a Hadamard gate operation on a qubit using Qiskit:

from qiskit import QuantumCircuit, Aer, execute

# Create a quantum circuit with one qubit
qc = QuantumCircuit(1)

# Apply the Hadamard gate to the qubit
qc.h(0)

# Simulate the circuit on a classical simulator
simulator = Aer.get_backend('statevector_simulator')
result = execute(qc, simulator).result()
statevector = result.get_statevector()

print("Statevector after applying H gate:", statevector)


NOT (X) Gate
The NOT gate is a basic quantum gate that flips the state of a qubit, transforming |0⟩ into |1⟩ and vice versa. The matrix representation of the NOT gate is:

X = [[0, 1], [1, 0]]



Implementation
The following Python code snippet demonstrates how to perform a NOT gate operation on a qubit using Qiskit:


from qiskit import QuantumCircuit, Aer, execute

# Create a quantum circuit with one qubit
qc = QuantumCircuit(1)

# Apply the NOT gate (X gate) to the qubit
qc.x(0)

# Simulate the circuit on a classical simulator
simulator = Aer.get_backend('statevector_simulator')
result = execute(qc, simulator).result()
statevector = result.get_statevector()

print("Statevector after applying X gate:", statevector)


markdown
Copy code
# Quantum Computer Operations

Welcome to the Quantum Computer Operations repository! This collection of code snippets demonstrates the implementation of basic quantum gate operations, including the Hadamard (H) gate and the NOT gate (also known as the X gate).

## Hadamard (H) Gate

The Hadamard gate is a fundamental quantum gate that creates superposition by transforming the basis states |0⟩ and |1⟩ into an equal superposition of both states. The matrix representation of the Hadamard gate is:

H = 1/√2 * [[1, 1], [1, -1]]

css
Copy code

### Implementation

The following Python code snippet illustrates how to perform a Hadamard gate operation on a qubit using Qiskit:

from qiskit import QuantumCircuit, Aer, execute

# Create a quantum circuit with one qubit
qc = QuantumCircuit(1)

# Apply the Hadamard gate to the qubit
qc.h(0)

# Simulate the circuit on a classical simulator
simulator = Aer.get_backend('statevector_simulator')
result = execute(qc, simulator).result()
statevector = result.get_statevector()

print("Statevector after applying H gate:", statevector)
NOT (X) Gate
The NOT gate is a basic quantum gate that flips the state of a qubit, transforming |0⟩ into |1⟩ and vice versa. The matrix representation of the NOT gate is:

lua
Copy code
X = [[0, 1], [1, 0]]
Implementation
The following Python code snippet demonstrates how to perform a NOT gate operation on a qubit using Qiskit:

python
Copy code
from qiskit import QuantumCircuit, Aer, execute

# Create a quantum circuit with one qubit
qc = QuantumCircuit(1)

# Apply the NOT gate (X gate) to the qubit
qc.x(0)

# Simulate the circuit on a classical simulator
simulator = Aer.get_backend('statevector_simulator')
result = execute(qc, simulator).result()
statevector = result.get_statevector()

print("Statevector after applying X gate:", statevector)
Getting Started
To run these code snippets:

Make sure you have Python and Qiskit installed on your system.

Copy and paste the code snippets into separate Python files.

Execute the Python files to see the statevector after applying the gate operations.

Contributing
Contributions to this repository are welcome! If you have additional quantum gate operations or improvements to the existing code snippets, feel free to submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
