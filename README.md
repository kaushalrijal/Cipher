# Caesar and Vigenere Encryption Algorithms

This repository contains Python implementations of two classic encryption algorithms: Caesar and Vigenere. These algorithms are used to encrypt and decrypt messages by shifting or substituting letters based on a given key.

## Caesar Cipher

The Caesar Cipher is a substitution cipher where each letter in the plaintext is shifted a certain number of places down or up the alphabet. In this implementation, the shift amount is provided as an offset.

### Usage

```python
text = 'Hello World'
shift = 3
# Encrypt message
encrypted = caesar(text, shift)
print(encrypted)  # Prints: 'khoor zruog'
# Decrypt message (optional)
decrypted = caesar(encrypted, -shift)
print(decrypted)  # Prints: 'hello world'
```

## Vigenere Cipher

The Vigenere Cipher is a method of encrypting alphabetic text using a simple form of polyalphabetic substitution. It uses a keyword to determine the shift amount for each letter in the plaintext.

### Usage

```python
text = 'q laol cul.'
custom_key = 'iamthegreat'
# Encrypt message
encrypted = encrypt(text, custom_key)
print(f'Encrypted text: {encrypted}')  # Prints: 'y xptk jmk.'
# Decrypt message
decrypted = decrypt(encrypted, custom_key)
print(f'Decrypted text: {decrypted}')  # Prints: 'i love you.'
```
