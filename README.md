## Number Theory and Cryptography (CO313)

### Mini Project

By: <br>
Mehnaz Yunus 16CO124 <br>
Sharanya Kamath 16CO140 <br>

### Modified RSA cryptosystem based on offline storage and prime number.

Paper Link: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6724176

### Abstract

This paper suggest a new algorithm concept
to presents the modified form of RSA algorithm in order to
speed up the implementation of RSA algorithm during data
exchange across the network. This includes the architectural
design and enhanced form of RSA algorithm through the use
of third prime number in order to make a modulus n which
is not easily decomposable by intruders

### Modified RSA Method
An algorithm is developed which is
based on modified RSA cryptosystem. Considering
these assumptions for algorithm-
 - p , q, and r are prime numbers.
 - n is common modulus.
 - e is public key.
 - d is private key.
 - M is message.

**RSA Proposed Method:** <br>
- Select the random values p, q, and r.
- Calculate n=p*q*r.
- Calculate Ø (n) = (p-1) (q-1) (r-1).
- Calculate e such that gcd (e, Ø(n))=1 and
1<e<Ø(n).
- Encrypt the message M where M<n and encrypt
with public key e such that C=M^e mod n.
- Calculate private key d = ℮-1 (mod Ø (n)).
- Decrypt the message M such that M=C^d
 mod n. 

### Requirements
- `python3`
- `pandas`

### How to run
`python3 modified-rsa.py`
