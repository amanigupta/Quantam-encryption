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
