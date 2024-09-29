## Quantum Encryption

As we stand on the cusp of the quantum computing era, traditional cryptographic systems face an unprecedented threat to their security. Quantum computers represent a serious threat to commonly used encryption techniques due to their capacity to execute intricate computations tenfold quicker than those of classical computers. This makes a large portion of the current cryptographic infrastructure susceptible to decoding attempts. 

Recognizing the imminent threat posed by the rapid development of quantum computing, this project aimed to design and rigorously test quantum-safe encryption algorithms. This work involved a comprehensive testing and evaluation framework for two existing quantum-safe encryption algorithms, as well as the development of a new algorithm, focusing on their security, efficiency, and practical applicability. A BIKC quantum encryption algorithm was created to compare against the Classic McEliece and BIKE methods. 

Through ANOVA analysis, BIKC demonstrated significantly higher levels of efficiency in encapsulation and decapsulation speeds (p > 0.01). However, a larger memory consumption was required to run the BIKC system. 

This work underscored the transformative potential of BIKC in securing digital communication, fostering trust, and inspiring future cryptographic innovations. Future research must emphasize the exploration of hybrid cryptographic protocols, practical implementations, interdisciplinary collaborations, and the evolution of post-quantum cryptography in the face of quantum threats.

### Review of Literature
Overview of Quantum Algorithms
The Classic McEliece, BIKE (Bit Flipping Key Encapsulation), and BIKC (Bit-Flipping Key Encapsulation influenced by BIKE) post-quantum code-based cryptography algorithms are all compared in-depth in this section. These algorithms are meant to be resistant to the potential risk that quantum computers bring to conventional cryptography techniques. To help stakeholders make wise choices about the adoption of Classic McEliece, BIKE, and BIKC for post-quantum cryptographic applications, this comparison analysis seeks to offer insightful information about the strengths and disadvantages of each algorithm. 

**Classic McEliece:** Robert McEliece first introduced Classic McEliece in 1978, and it is a strong contender for NIST's global standardization. It has changed very little throughout time, with the main goal being to improve computing efficiency. All five NIST security levels can be adjusted for using the standard McEliece parameters. Notably, despite requiring a big public key size, it offers astonishing computing performance. 

**BIKE (Bit Flipping Key Encapsulation):** BIKE uses bit flipping decoding along with quasi-cyclic moderate density parity-check (QC-MDPC) codes. In order to adhere to NIST security levels 1 and 3, it was specifically designed. BIKE offers a fascinating replacement for Classic McEliece, utilizing its distinct decoding strategy to improve post-quantum security. 

**BIKC (Bit-Flipping Key Encapsulation inspired by BIKE):** The BIKE algorithm serves as the basis for BIKC, also known as Bit-Flipping Key Encapsulation inspired by BIKE. BIKC is built to achieve NIST security levels 1, 3, and 5 and is intended to offer strong protection against both classical and quantum computers. By drawing inspiration from the ground-breaking BIKE algorithm, BIKC offers a flexible solution for post-quantum cryptography requirements.


### Post Quantum Cryptography
	Post-quantum cryptography has advanced significantly in recent years as academics work to create encryption algorithms that can withstand quantum attacks, Figure 1 shows some examples. Lattice-based cryptography, code-based cryptography, hash-based cryptography, multivariate polynomial cryptography, and other strategies have all been investigated, according to the literature review (Kostic et al., 2020). These techniques provide intriguing post-quantum security options since they are based on mathematical constructs that seem difficult for quantum computers to decipher. To find the best strategies and enhance these algorithms' performance, more investigation is necessary.

![Figure 1: Examples of Algorithms (NIST, 2022)](https://github.com/amanigupta/Quantum-encryption/blob/main/1.jpg)


The requirement for uniform assessment frameworks is an important factor in the development of quantum-safe encryption. To evaluate and standardize quantum-resistant encryption techniques, the National Institute of Standards and Technology (NIST) launched the Post-Quantum Cryptography Standardization process (NIST, 2022). As part of this continuous endeavor, proposed algorithms are rigorously assessed and put through public competitions to make sure they are resilient to quantum assaults. NIST wants to encourage the wide adoption and interoperability of quantum-safe encryption technologies by creating standards.
	While encouraging, the current research also highlights weaknesses and difficulties in quantum-safe encryption. When used in real-world circumstances, several encryption algorithms may have attractive security characteristics yet have performance issues. Making effective post-quantum cryptography algorithms still requires careful consideration of how to strike a balance between security and efficiency. Additionally, due to the dynamic nature of quantum computing, quantum-safe encryption must constantly be evaluated for its resistance to new quantum algorithms.

![Figure 2: Quantum Key Decryption (Sullivan, 2013)](https://github.com/amanigupta/Quantum-encryption/blob/main/2.jpg)


	The security issues raised by quantum computing have given rise to a ground-breaking solution known as quantum encryption, commonly referred to as quantum key distribution shown in figure 2 (QKD). Quantum encryption, in contrast to classical encryption, which depends on mathematical difficulty, uses the concepts of quantum mechanics to provide complete security (Kumar, 2022). Quantum encryption provides a fundamentally secure method of exchanging cryptographic keys between parties by encoding information in quantum states, such as polarized photons. Any attempt to intercept or measure quantum states would disrupt the communication, revealing the presence of an attacker, it is noteworthy that quantum encryption offers protection against eavesdropping.
Quantum Entanglement

	The investigation of entanglement-based protocols is another important development in quantum encryption. New opportunities for 
 
cryptography applications are presented by quantum entanglement, a phenomenon where the quantum states of two or more particles start to depend on one another. Quantum Entanglement Decryption (QKD) algorithms take advantage of this non-classical correlation to improve the security of quantum key distribution (Sullivan, 2013). Technology challenges, such as the creation and

maintenance of entangled states under actual environmental conditions, must be overcome before entanglement can be effectively used in practical quantum communication systems.

	An advancement in addressing the difficulties of long-distance quantum communication is the use of quantum repeaters. By dividing the link into smaller segments and subsequently entangling them, quantum repeaters enable the dispersion of entanglement over long distances (Kumar, 2022) Quantum repeaters reduce the impacts of quantum channel loss and decoherence by using quantum error. 
 
correction methods and quantum memory, making long-range quantum communication a practical possibility. Although this technology is still going through its developmental phases, the proposed technology seems similar to the one implemented in our research.

![Figure 2: Quantum Key Decryption (Sullivan, 2013)](https://github.com/amanigupta/Quantum-encryption/blob/main/3.jpg)

	To complete this research, numerous post-quantum cryptographic algorithms were assessed according to their security and effectiveness characteristics. Phase two builds on this foundation by identifying limits and refining the chosen algorithms for application in practice. The algorithms will be adjusted, improvements will be made, and extensive benchmarking will be done to assess how well they function in practical settings. The project will also look at potential integration issues and investigate approaches to easily integrate quantum-safe encryption into current infrastructures and systems.

### Problem Statement(s):
P1: The challenge is to develop comprehensive testing methodologies that rigorously assess existing quantum-safe encryption algorithms, identifying potential vulnerabilities and weaknesses, to enhance their security levels and ensure resilience against quantum attacks.



### Objective(s): 
O1: Develop an algorithm testing for existing quantum computers that work more efficiently than    already existing quantum-safe algorithms. 
Develop a new system that improves security levels against quantum attacks upon the foundations of the existing BIKC system.
Successfully run the quantum-safe encryption algorithm on the quantum computer while retaining accurate results.
By subjecting these algorithms to a range of security analyses, the research aims to compare Classic McEliece, BIKE, and BIKC in encapsulation and decapsulation speeds, as well as test their memory consumption.

### Hypothesis: 
H: Improving the testing and implementation of quantum-safe encryption algorithms on real quantum computers, particularly by refining the BIKC system, will enhance security and resilience against quantum attacks, achieving faster speeds, lower memory consumption, and accurate results compared to Classic McEliece and BIKE.


### Methodology: 
#### Algorithm Selection and Setup 
The first step involves selecting Classic McEliece and BIKE from the open-source C library for quantum-safe cryptographic algorithm (liboqs) library. Classic McEliece was chosen for its historical significance and established status as a benchmark in post-quantum cryptography. BIKE, a pr
omising code-based algorithm, was selected for its unique bit-flipping decoding strategy. Subsequently, BIKC is conceptualized as an extension of BIKE, combining its innovative features with additional enhancements. The chosen algorithms are then implemented using the Python programming language within the framework for quantum computing simulations.

![Figure 2: Quantum Key Decryption (Sullivan, 2013)](https://github.com/amanigupta/Quantum-encryption/blob/main/4.jpg)

#### Identifying Areas for Improvement in the BIKE Algorithm
To identify potential areas for improvement in the BIKE algorithm, we conducted a comprehensive analysis focusing on its performance, security, and efficiency. The performance analysis involved benchmarking the algorithm under various scenarios to measure execution time, memory usage, and computational efficiency. Security analysis was carried out to assess the algorithm's resilience against known quantum and classical attacks, evaluating its robustness in encryption and decryption processes. By examining these metrics, we identified specific vulnerabilities and weaknesses that could be addressed to enhance the algorithm's overall performance and security.

##### Refining the BIKC Algorithm
To enhance the BIKE algorithm's security and performance, we brainstormed potential modifications, including changes to parameters, key generation techniques, and encryption/decryption processes. These modifications were aimed at improving the algorithm's resistance to quantum attacks. We then implemented the modified algorithm in Qiskit, a quantum programming language compatible with our target quantum computer. The algorithm was translated into quantum circuit representations using Qiskit's syntax, ensuring that it adhered to the necessary quantum computing principles.

#### Testing and Adapting Algorithm
Before testing the modified algorithm on quantum hardware, we verified its functionality and correctness using classical computers. Classical simulators were employed to test the algorithm's performance, measuring its speed and resource consumption. This step was crucial to ensure that the algorithm performed as expected and to identify any issues that could be addressed before quantum implementation.
To adapt the algorithm for quantum computing, we optimized it for quantum gates and qubit operations. This involved modifying the algorithm to use suitable quantum gates and optimizing the quantum circuit representation for efficient execution on quantum hardware. The adapted algorithm was then prepared for execution on the target quantum computer, with the quantum circuit representing the modified BIKE algorithm being submitted for encapsulation and decapsulation tasks. We specified the required inputs for these processes and ran the algorithm on the quantum computer.


#### Analysis and Iteration
After running the adapted algorithm on the quantum computer, we collected the output and compared the results with expected outcomes to verify correctness. We assessed the algorithm's performance metrics, such as speed and resource usage, using statistical analysis methods, including ANOVA, to evaluate the significance of our modifications. Based on this analysis, we iterated on the modifications to further enhance the algorithm, considering additional changes and optimizations to address any identified issues or shortcomings. This iterative process aimed to continually improve the BIKE algorithm's efficiency, security, and resilience against quantum attacks.

