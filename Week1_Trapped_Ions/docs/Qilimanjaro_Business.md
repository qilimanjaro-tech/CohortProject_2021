![CDL 2021 Cohort Project](./images/logo.jpg)
# rQIBO: assessing quantum computers with randomized benchmarking

## Step 1: Explain the technical problem you solved in this exercise

Identifying proper metrics and benchmarks to assess the quality of quantum devices is paramount in the development of quantum computation. In order to ensure the correcteness of any computation, quantum devices need to be calibrated before running any algorithm. However the quantum nature of the device sets a fundamental limitation and as its size increases the number of measurements that full-tomography would require to characterize noise makes this method highly unpractical. 

Random quantum circuits have been widely implemented in superconducting qubit chips but so far its reach has been limited to proofs of concept in quantum advantage experiments. We here propose **rQibo**: a library based on [Qibo](https://qibo.readthedocs.io/) with a full-stack implementation of randomized benchmarking, a protocol that allows the use of such circuits as benchmarks, to assess the capabilities of superconducting NISQ devices. 

In randomized benchmarking a random circuit composed of one- and two-qubit Clifford gates is concatenated with its reverse (conjugate transpose) to an initial state with all qubits in the 0 (or down) state. In the absence of errors, this effectivly applies a random quantum operation to the qubits and undoes it afterwards. The consequence of this is that the final state is equal to the initial one. However, if errors happen the initial and final state are not the same. Under this framweork, sampling the output state probabilities of random circuits of different depths gives information on the present errors. 

<img src="./images/randbench.png" width="500">

## Step 2: Explain or provide examples of the types of real-world problems this solution can solve


## Step 3: Identify at least one potential customer for this solution - ie: a business who has this problem and would consider paying to have this problem solved
## Step 4: Prepare a 90 second video explaining the value proposition of your innovation to this potential customer in non-technical language
