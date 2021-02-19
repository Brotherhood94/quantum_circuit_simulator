# Quantum Circuit Simulator
### The assumptions made are:
- Given a generic gate and "n" target_quibits, the first "n-1" qubits are control qubits, while the last is the target qubit.
- Any unitary gate, which has a number of target_qubits > 1, is a controlled gate.
    - Example: {'gate': 'x', 'target': '[0,1]'} it is intepred as a X gate whose control qubit is 0 and target qubit is 1 (CX)
    - {'gate': 'x', 'target': '[0,1,2]'}, follows the same logic, thus it is a Toffoli gate
