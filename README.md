# RSA Algorithm Visualization

A simple implementation of the RSA Algorithm written in Python 3 with GUI implemented with Tkinter.

## Algorithm
The algorithm you provided is an implementation of the RSA (Rivest-Shamir-Adleman) encryption and decryption scheme. Here's a simplified version of the algorithm:

1. **Key Generation**:
   - Choose two distinct prime numbers, \( p \) and \( q \).
   - Compute \( n = p \times q \).
   - Calculate Euler's totient function: \( \phi(n) = (p-1) \times (q-1) \).
   - Choose an integer \( e \) such that \( 1 < e < \phi(n) \) and \( e \) is coprime with \( \phi(n) \), i.e., \( \text{gcd}(e, \phi(n)) = 1 \).
   - Compute \( d \), the modular multiplicative inverse of \( e \) modulo \( \phi(n) \), i.e., \( d \times e \equiv 1 \pmod{\phi(n)} \).
   - The public key is \( (e, n) \), and the private key is \( (d, n) \).

2. **Encryption**:
   - Represent the plaintext message as integers \( m \), where \( 0 \leq m < n \).
   - Encrypt each integer \( m \) using the public key \( (e, n) \): \( c \equiv m^e \pmod{n} \).

3. **Decryption**:
   - Decrypt the ciphertext \( c \) using the private key \( (d, n) \): \( m \equiv c^d \pmod{n} \).

4. **Prime Factorization**:
   - This function finds the prime factors of a given number \( n \).

5. **Helper Functions**:
   - Various helper functions like checking if a number is prime, generating key pairs, and getting encrypted string representations are provided.

## Tkinter UI 
This program offers a straightforward GUI interface for users to interactively explore and understand the RSA encryption and decryption process, facilitating message input, encryption, and visualization of the encryption and decryption steps.

## Contributors

* Adithya
* Maran
