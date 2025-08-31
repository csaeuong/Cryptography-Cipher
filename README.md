# Cryptography-Cipher

## Objective

The objective of this project is to implement a classic Caesar Cipher in Python that can both encrypt and decrypt messages. This project demonstrates how substitution ciphers work by shifting letters of the alphabet by a fixed key value. It is a fundamental introduction to cryptography and shows how simple algorithms can protect (and expose) information.

### Skills Learned

- Python programming fundamentals (functions, user input, string manipulation)
- Understanding of encryption and decryption logic
- Working with built-in Python libraries (string for alphabets, str.maketrans and .translate for substitutions)
- Application of the modulo operator to ensure cyclic shifts in the alphabet
- Designing a basic command-line interface for user interaction
- Differentiating between encryption and decryption operations

### Tools Used

- Python 3 (main programming language)
- string (for accessing predefined lowercase alphabets)
- str.maketrans() and translate() (for letter substitution logic)

## Code 

<img width="1920" height="1040" alt="Cryptography Cipher" src="https://github.com/user-attachments/assets/6a8ffb54-a337-4cab-b8d1-02b1027fe973" />


### Quick Reference

- import string – loads Python’s string library for easy access to lowercase alphabets.
- def caesar_encrypt(message, key): – defines the encryption function.
- shift = key % 26 – ensures the key always cycles through the 26 letters of the alphabet.
- str.maketrans(...) – builds a mapping of original letters to shifted letters.
- message.lower().translate(cipher) – converts the message to lowercase and applies substitution.
- def caesar_decrypt(encrypted_message, key): – defines the decryption function.
- shift = 26 - (key % 26) – reverses the shift to recover the original message.
- input("Type your message: ") – asks the user for a message.
- int(input("Enter your key: ")) – takes the encryption key from the user.
- print(f'Encrypted message: {encrypted_message}') – outputs the encrypted text.
- print(f'Decrypted message: {decrypted_message}') – outputs the original text after decryption.

## Project Reflection

I learned a lot while working on this project. It helped me understand the foundations of cryptography and how even a simple algorithm like the Caesar Cipher works behind the scenes. I had to research concepts like character shifting, translation tables, and modular arithmetic to fully grasp how the code functioned.  

Although this is a very basic form of encryption, it showed me how important logic and precision are when working with security-related code. This project also gave me practice with Python functions, user input, and string manipulation, which are skills I can apply to more advanced projects in the future.  

One of the small but important challenges I ran into was figuring out that the input() function in Python always returns a string, even if the user types a number. At first, this caused errors when I tried to use the key in mathematical operations like % 26. The solution was to explicitly convert the input into an integer using int(input(...)). It seems like a small fix, but it taught me an important lesson about data types in Python and how user input is handled.
