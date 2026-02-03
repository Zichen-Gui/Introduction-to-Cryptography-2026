# CSCI 4900/6900 Introduction to Cryptography
Welcome to the course repository of CSCI 4900/6900 Introduction to Cryptography! You can find an overview of the course below (updated weekly). The programming exercises of the course are in the `Labs` folder.

We are using the book "A Gruaduate Course in Applied Cryptography" by Dan Boneh and Victor Shoup as the reference.
https://toc.cryptobook.us/


## Lectures
| Lecture | Topic(s) | Remarks |
|---------|----------|---------|
| 1       | - Shannon cipher and perfect security <br> - Semantic security | - Boneh & Shoup 2.1-2.2     |
| 2       | - How to prove that a scheme is semantically secure <br> - How to attack an insecure cipher |      |
| 3       | - Pseudorandom generators | - Boneh & Shoup 3.1-3.2 <br> - Exercise 3.7 <br> - [Breaking Go Ethereum by exploiting the weak PRG in its implementation](https://www.usenix.org/conference/usenixsecurity23/presentation/taverna) |
| 4       | - Security of stream cipher <br> - Composing PRGs | - Boneh & Shoup 3.3, 3.4   |
| 5       | - Linear congruential generator <br> - CSS stream cipher <br> - Commitment scheme from PRG | - Boneh & Shoup 3.7.1, 3.8, 3.12 <br> - [An entertaining video on how to break Math.random()](https://www.youtube.com/watch?v=XDsYPXRCXAs)   |
| 6,7     | - Pseudorandom functions (PRFs) | - Boneh & Shoup 4.4 <br> - Exercise 4.1  |
| 8       | - From PRGs to PRFs <br> - Constrained PRFs <br> - An application of PRFs: searchable symmetric encryption (SSE) | - Boneh & Shoup 4.6 <br> - [Constrained Pseudorandom Functions and Their Applications](https://eprint.iacr.org/2013/352) <br> -[Adaptive Security for Constrained PRFs](https://eprint.iacr.org/2025/2122) (with applications in SSE) |
| 9       | - Block ciphers (a.k.a. pseudorandom permutations) <br> - PRF switching lemma <br> - DES and its variants | - Boneh & Shoup 4.1, 4.2, 4.4.3   |




## Labs
| Lab | Topic(s)                                       | Remarks |
|-----|------------------------------------------------|---------|
| 1   | - Implement One-Time Pad <br> - Attack Two-Time Pad |         |
| 2   | - Attack `Math.random()` in Java 8 <br> - Implement the Content Scrambling System (CSS). <br> - Attack CSS |         |
| 3   | - Implement FEAL <br> - Attack FEAL | -  [Akihiro Shimizu, Shoji Miyaguchi. Fast Data Encipherment Algorithm FEAL.](https://link.springer.com/chapter/10.1007/3-540-39118-5_24) <br> - [Mitsuru Matsui, Atsuhiro Yamagishi. A New Method for Known Plaintext Attack of FEAL Cipher](https://link.springer.com/chapter/10.1007/3-540-47555-9_7) |




## Examinable Material
### 0. General Techniques
- Prove that a simple scheme is secure with respect to a security notion.
- If a scheme is not secure with respect to a security notion, show a concrete attack against the security notion
- Given a scheme, analyze its efficiency. For example, the number of keys required for the scheme, the number of PRF evaluations needed by the scheme, for an encryption scheme, whether the encryption/decryption can be parallelized, and so on.



### 1. Encryption
- Definition of Shannon cipher.
- Definition of perfect security.
- One-time pad and its limitations.
- Given that $\mathcal{E}$ is semantically secure, prove that $\mathcal{E}'$ (that is a simple variant of $\mathcal{E}$) is (or is not) semantically secure.


### 2. Stream Ciphers
- Definition of PRG and PRG security.
- Given that $G$ is a secure PRG, prove (or disprove) that $G'$ (that is a simple variant of $G$) is a secure PRG.
- Reproduce the parallel and sequential compositions of PRGs. Informally argue about their security.


### 3. Block Ciphers
- Definition of block cipher and its security.
- Definition of pseudo-random function (PRF) and its security.
- PRF switching lemma.
- Deterministic counter mode.
