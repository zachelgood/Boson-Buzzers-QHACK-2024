**QHack Open Hackathon 2024**

# :space_invader: Seeing the future challenge- Team Boson Buzzers

- [Team Introduction](#team-introduction)
- [Problem Statement](#ProblemStatement)
  - [Description](#description)
- [Results](#Results)
- [Software & Tools Used](#software--tools-used)
- [Future Plans](#future-plans)
- [License](#license)
- [Acknowledgement](#Acknowledgement)
- [References](#references)

## Team Introduction
**Team Name:** Boson Buzzers

**Challenge Name:** Seeing the future



****Member Names:****

------------

**Abdullah Kazi**

Discord ID: **Maddy**

GitHub ID: **AbdullahKazi500**

 
------------


**Bakhao Dioum**


Discord ID: Bakhao


GitHub ID: papidioum



------------

**Zach Elgood**


Discord ID: timpinen


GitHub ID: zachelgood


------------

**Aakash Warke**


Discord ID: 

------------



## Problem Statement
One of the tasks in which a quantum computer is expected to excel compared to a classical one is the simulation of quantum systems. The dynamics of a quantum system are usually represented by its Hamiltonian H. The complex exponential of the Hamiltonian:

$$U=e^{-iHt}$$

is a very useful operator because it calculates how the system evolves over time. The construction of this operator is usually done through Trotter methods or more modern techniques such as QDrift. Your goal will be to implement state-of-the-art ways to construct the complex exponential of the Hamiltonian, or invent a new original way to achieve this task. Note that there are also more complex Hamiltonians that are time dependent where you could provide different techniques.

This evolution operator has many applications in different fields as chemistry or optimization tasks, it would be great if you could help us!
## Description 
In this project, we examine an alternative to the Trotter decomposition to estimate the time evolution of a time independent Hamiltonian. This is accomplished through the use of a method known as Cartan decomposition, a procedure by which we can decompose a Hamiltonian algebra into smaller subalgebras. To accomplish this, we shall follow the procedure implemented in \cite{ref1}, utilizing their Cartan Quantum Synthesizer (CQS) program\cite{ref2}. We apply this to three different molecules: $H_2$, $HeH^+$, and $BeH_2$ with 2 active orbitals. For detailed information as to how Cartan decomposition works, please see the pdf included as well as the relavent notebooks. 
## Results
For detailed results about each individual molecule, see their respective Jupyter notebook. 

In this project, we have illustrated that through the use of Cartan decomposition, we can produce a significantly smaller error with respect to the exact Unitary compared to the error associated with the Trotter decomposition. This implies that theoretically, we could lower the depth of the Cartan decomposition even further if we were content with a higher error.

## software--tools-used
[_Pennylane SDK_](https://pennylane.ai/)

[Cartan Quantum Synthesizer](https://github.com/kemperlab/cartan-quantum-synthesizer)
## Future Work
While we have applied this Cartan decomposition to three different molecules( $H_2$, $HeH^+$, and $BeH_2$ with 2 active orbitals), there is theoretically no issue with its implementation in other molecules, while noting that increased qubits would increase the processing time of the classical part of the algorithm, a.k.a. finding the parameters of the Cartan decomposition. Further work could involve optimizing the code to improve the efficiency of that part for a higher number of qubits. 
## License

<a href="https://choosealicense.com/licenses/mit/"><img src="https://raw.githubusercontent.com/johnturner4004/readme-generator/master/src/components/assets/images/mit.svg" height=40 />MIT License</a>

## Acknowledgement 
## References
