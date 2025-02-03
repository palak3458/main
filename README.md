Text Processing and Encryption Library
This library provides various functions for text processing and encryption, including text stripping, letter distribution analysis, substitution cipher encryption and decryption, Vigenère cipher encryption and decryption, and cryptanalysis of substitution and Vigenère ciphers.

Functions
1. textstrip(f)
This function reads a text file, converts it to a string, removes all spaces and special characters, and retains only the lowercase letters.

Parameters: f (str) - the filename of the text file to be processed.
Returns: A string containing only the lowercase letters from the original text.
2. letter_distribution(s)
This function takes a string of lowercase letters and returns a dictionary with the count of each letter.

Parameters: s (str) - the input string.
Returns: A dictionary with letters as keys and their counts as values.
3. substitution_encrypt(s, d)
This function encrypts a string using a substitution cipher based on a given dictionary of letter substitutions.

Parameters:
s (str) - the input string.
d (dict) - a dictionary with substitutions for each letter.
Returns: The encrypted string.
4. substitution_decrypt(s, d)
This function decrypts a string encrypted with a substitution cipher using a given dictionary of letter substitutions.

Parameters:
s (str) - the encrypted string.
d (dict) - a dictionary with substitutions for each letter.
Returns: The decrypted string.
5. cryptanalyse_substitution(s)
This function attempts to decrypt a string encrypted with a substitution cipher by using the frequency analysis of letters.

Parameters: s (str) - the encrypted string.
Returns: A dictionary with predicted substitutions for each letter.
6. vigenere_encrypt(s, password)
This function encrypts a string using the Vigenère cipher and a given password.

Parameters:
s (str) - the input string.
password (str) - the password for encryption.
Returns: The encrypted string.
7. vigenere_decrypt(s, password)
This function decrypts a string encrypted with the Vigenère cipher using a given password.

Parameters:
s (str) - the encrypted string.
password (str) - the password for decryption.
Returns: The decrypted string.
8. rotate_compare(s, r)
This function rotates a string by a given number of places and compares the original string with the rotated string to calculate the proportion of collisions.

Parameters:
s (str) - the input string.
r (int) - the number of places to rotate.
Returns: The proportion of collisions.
9. cryptanalyse_vigenere_afterlength(s, k)
This function attempts to find the password used to encrypt a string with the Vigenère cipher, given the length of the password.

Parameters:
s (str) - the encrypted string.
k (int) - the length of the password.
Returns: The decrypted password.
10. cryptanalyse_vigenere_findlength(s)
This function attempts to find the length of the password used to encrypt a string with the Vigenère cipher.

Parameters: s (str) - the encrypted string.
Returns: The length of the password.
11. cryptanalyse_vigenere(s)
This function attempts to decrypt a string encrypted with the Vigenère cipher by first finding the length of the password and then the password itself.

Parameters: s (str) - the encrypted string.
Returns: The decrypted plaintext.
Example Usage
Python
import string

# Example to strip text, analyze letter distribution, and encrypt/decrypt using substitution cipher
text = textstrip('english_random.txt')
letter_dist = letter_distribution(text)
substitution_key = {'a': 'm', 'b': 'n', 'c': 'o', 'd': 'p', 'e': 'q', 'f': 'r', 'g': 's', 'h': 't', 'i': 'u', 'j': 'v', 'k': 'w', 'l': 'x', 'm': 'y', 'n': 'z', 'o': 'a', 'p': 'b', 'q': 'c', 'r': 'd', 's': 'e', 't': 'f', 'u': 'g', 'v': 'h', 'w': 'i', 'x': 'j', 'y': 'k', 'z': 'l'}
encrypted_text = substitution_encrypt(text, substitution_key)
decrypted_text = substitution_decrypt(encrypted_text, substitution_key)

# Example to encrypt/decrypt using Vigenère cipher
password = "arunima"
vigenere_encrypted = vigenere_encrypt(text, password)
vigenere_decrypted = vigenere_decrypt(vigenere_encrypted, password)ere 👋

<!--
**palak3458/palak3458** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
