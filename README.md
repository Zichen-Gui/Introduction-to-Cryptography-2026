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
| 8       | - From PRGs to PRFs <br> - Constrained PRFs <br> - An application of PRFs: searchable symmetric encryption (SSE) | - Boneh & Shoup 4.6 <br> - [Constrained Pseudorandom Functions and Their Applications](https://eprint.iacr.org/2013/352) <br> - [Adaptive Security for Constrained PRFs](https://eprint.iacr.org/2025/2122) (with applications in SSE) |
| 9       | - Block ciphers (a.k.a. pseudorandom permutations) <br> - PRF switching lemma <br> - DES and its variants | - Boneh & Shoup 4.1, 4.2, 4.4.3   |
| 10       | - Chosen plaintext attack (CPA) <br> - Generic hybrid construction <br> - Randomized counter mode <br> - Randomized CBC mode | - Boneh & Shoup 5.1-5.5   |
| 11      | - Message authentication codes (MACs) <br> - MAC from PRF | - Boneh&Shoup 6.1-6.3  |
| 12      | - CBC prefix-free PRF and cascade prefix-free PRF <br> - Encrypted CBC/cascade MACs <br> - Prefix-free encoding <br> - Randonmized prefix-free encoding | - Boneh&Shoup 6.4-6.7 |
| 13      | - Insecure variants of CBC MAC <br> Bit-wide PRF <br> - CMAC <br> - PMAC | - Boneh&Shoup 6.4, 6.10-6.11 <br> - Exercise 6.8, 6.9  |
| 14      | - Universal hashing <br> - PRF(UHF) composition <br> - Polynomial hash | - Boneh&Shoup 7.1-7.3  |
| 15      | - Polynomial hash <br> - Carter-Wegman MAC | - Boneh&Shoup 7.2, 7.4  |
| 16      | - Carter-Wegman MAC (continued) | - Boneh&Shoup 7.4  |
| 17      | - Nonce-based MACs <br> - Unconditionally secure one-time MACs | - Boneh&Shoup 7.5, 7.6 |
| 18      | - Collision resistant hash <br> - Other applications of CR hash <br> - Birthday attacks <br> - The Merkle-Damgard paradigm | - Boneh&Shoup 8.1-8.4, 8.9 |
| 19      | - Building compression functions <br>  - HMAC <br> - The sponge construction<br> - Password hashing | - Boneh&Shoup 8.5, 8.7, 8.8, 18.3, 18.4 |
| 20      | - Authenticated encryption | - Boneh&Shoup 9.1-9.4 |
| 21      | - Authenticated encryption (continued) | - Boneh&Shoup 9.5, 9.7, 9.10 |
| 22      | - Overview of public key cryptography | |
| 23      | - Introduction to groups | - [Group on Wikipedia](https://en.wikipedia.org/wiki/Group_(mathematics)) |
| 24      | - Introduction to groups (continued) <br> - Exponentiation by squaring <br> - Diffie-Hellman key exchange <br> - Man-in-the-Middle attack against DHKE| - [Group on Wikipedia](https://en.wikipedia.org/wiki/Group_(mathematics)) <br> - [Exponentiation by squaring](https://en.wikipedia.org/wiki/Exponentiation_by_squaring) <br> - Boneh & Shoup 10.4, 10.7 |
| 25      | - Diffie-Hellman key exchange, concretely ([RFC 2631](https://datatracker.ietf.org/doc/html/rfc2631)) <br> - Miller–Rabin primality test <br> - Baby-step giant-step | - [Why 2048-bit prime p?](https://weakdh.org/imperfect-forward-secrecy-ccs15.pdf) <br> - [Why (at least) 256-bit prime q?](https://en.wikipedia.org/wiki/Baby-step_giant-step) <br> - [Miller–Rabin primality test](https://en.wikipedia.org/wiki/Miller–Rabin_primality_test) <br> - Boneh & Shoup 16.1 |
| 26      | - RSA <br> - RSA accumulator | - Boneh & Shoup 10.3, 10.9 |
| 27      | - Semantic security and CPA <br> - Encryption based on a trapdoor function scheme <br> - ElGamal encryption <br> - Oblivious transfer based on Diffie-Hellman | - Boneh&Shoup 11.2-11.6 |
| 28      | - CCA <br> - PKCS1 <br> - OAEP <br> - Oblivious PRFs | - Boneh&Shoup 12.1-12.4, 12.8 <br> - [OPRF](https://eprint.iacr.org/2014/650) |






## Labs
| Lab | Topic(s)                                       | Remarks |
|-----|------------------------------------------------|---------|
| 1   | - Implement One-Time Pad <br> - Attack Two-Time Pad |         |
| 2   | - Attack `Math.random()` in Java 8 <br> - Implement the Content Scrambling System (CSS). <br> - Attack CSS |         |
| 3   | - Implement FEAL <br> - Attack FEAL | -  [Akihiro Shimizu, Shoji Miyaguchi. Fast Data Encipherment Algorithm FEAL.](https://link.springer.com/chapter/10.1007/3-540-39118-5_24) <br> - [Mitsuru Matsui, Atsuhiro Yamagishi. A New Method for Known Plaintext Attack of FEAL Cipher](https://link.springer.com/chapter/10.1007/3-540-47555-9_7) |
| 4   | - Differential fault analysis of AES | - [Michael Tunstall, Debdeep Mukhopadhyay, Subidh Ali. Differential Fault Analysis of the Advanced Encryption Standard using a Single Fault](https://eprint.iacr.org/2009/575) |
| 5   | - Implement a padding oracle attack on AES-CBC (GRADED) |         |
| 6   | - Collision attacks against MD4 and MD5 | - [X. Wang, X. Lai, D. Feng, H. Chen and X. Yu. Cryptanalysis of the Hash Functions MD4 and RIPEMD. Eurocrypt 2005.](https://www.iacr.org/archive/fse2007/45930331/45930331.pdf) <br> - [M. Schl¨affer and E. Oswald. Searching for Differential Paths in MD4. Fast Software Encryption (FSE) 2006.](https://www.iacr.org/archive/fse2006/40470245/40470245.pdf) <br> - [Y. Sasaki, L. Wang, K. Ohta and N. Kunihiro. New Message Difference for MD4. Fast Software Encryption (FSE) 2007.](https://iacr.org/archive/fse2007/45930331/45930331.pdf)        |
| 7   | - Chopchop attack against 802.11b WEP | - [M. Guennoun, A. Lbekkouri, A. Benamrane, M. Ben-Tahir and K. El-Khatib, "Wireless networks security: Proof of chopchop attack," 2008 International Symposium on a World of Wireless, Mobile and Multimedia Networks.](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=4594924)  |
| 8   | - Implement Diffie-Hellman Key Exchange | - [RFC 2631](https://datatracker.ietf.org/doc/html/rfc2631) |
| 9   | - Implement RSA cryptosystem |         |
| 10  | - Implement the Pohlig-Hellman Algorithm (GRADED) |         |




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
- Given that F is a secure PRF, prove (or disprove) that F' is a secure PRF.
- PRF switching lemma.
- Deterministic counter mode.


### 4. Chosen Plaintext Attack
- Definition of CPA security.
- Generic hybrid construction.
- Randomized counter mode and randomized CBC mode.


### 5. Message Integrity
- Definition of MAC security.
- MAC from PRF.
- Prefix-free PRFs: the CBC construction and the nested construction.
- Insecure variants of the CBC construction and the nested construction.


### 6. Message Integrity from Universal Hashing
- UHF and PRF(UHF) compositon
- DUF and the Carter-Wegman MAC
- PUF and unconditionally secure one-time MACs


### 7. Message Integrity from Collision Resistant Hashing
- Definition of collision resistant hashing
- Hash-then-MAC paradigm
- Birthday attack on collision resistant hash functions
- The Merkle-Damgard paradigm
- Davies-Meyer compression functions


### 8. Authenticated Encryption
- Definition of ciphertext integrity
- Definition of authenticated encryption
- Nonce-based authenticated encryption with associated data
- Generic compositions: MAC-then-encrypt and encrypt-then-MAC
