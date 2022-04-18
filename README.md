# Enigma-Machine

# Background 
The Enigma machine is a cipher device developed and used in the early- to mid-20th century to protect commercial, diplomatic, and military communication. It was employed extensively by Nazi Germany during World War II, in all branches of the German military. The Enigma machine was considered so secure that it was used to encipher the most top-secret messages. The Enigma has an electromechanical rotor mechanism that scrambles the 26 letters of the alphabet. In typical use, one person enters text on the Enigma's keyboard and another person writes down which of the 26 lights above the keyboard illuminated at each key press. If plain text is entered, the illuminated letters are the encoded ciphertext. Entering ciphertext transforms it back into readable plaintext. The rotor mechanism changes the electrical connections between the keys and the lights with each keypress.


# Encryption 

Enigma machine uses rotors to encrypt messages. Inside the code for enigma_driver.c there is an array of strings called ROTOR_CONSTANTS that stores nine rotors. For our project, the rotor at position 0 is an identity rotor. It is a string with original English alphabets in the correct order.
Choose which rotors to use and in what order they will be applied. 

Rotate the letters in each rotor. For each letter of the message, find the position in the identity rotor and look up the letter at the same position in the encryption rotors. Then repeat with all of the other rotors.

# Decryption 

To decrypt an encoded message we just apply the rotors in the reverse order.  Look up the letter in the encryption rotor, find its position then look up the letter at that position in the identity rotor.  Then repeat with the other rotors.  In the above example, we find the letter P in rotor 1 at position 19 then look up the letter at position 19 in the identity rotor, T.  Then apply rotor 3. Find the letter T and look up the letter at the same position in the identity rotor.

# Rotating Rotors
Enigma machines also have the ability to change the letters in each encryption rotor by shifting all of the letters to the right. This is a cyclic shift.  For example, consider rotor 1 with 3 rotations applied to it.

Rotor 1 – EKMFLGDQVZNTOWYHXUSPAIBRCJ (before rotations)
Rotor 1 – RCJEKMFLGDQVZNTOWYHXUSPAIB (after 3 rotations)


# Test Case:
```Message: JAVA
Rotors to use: 31
Number of rotations: 0
Encrypted message: PKOK
Decrypted message: JAVA
```

# Learning Goals
1. Learn how to write a C program that follows the given specifications.
2. Learn how functions improve code by making it modular and task-oriented.
3. Practice calling functions from different functions.
4. Practice passing arguments to functions.
5. Practice returning values from functions.
6. Develop code using one-dimensional and two-dimensional arrays.
7. Learn to write code that follows the commenting and the style guidelines. 
