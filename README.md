# DES

This project implements the Data Encryption Standard (DES) algorithm in C. It provides functionality for encryption and decryption of data using DES, along with test cases to validate the implementation.

## File Descriptions
### [main.c](main.c)

This file contains the implementation of the DES algorithm, including:

- **Key Scheduling**:
  - `deskey`: Sets the internal key register for encryption or decryption.
  - `cookey`: Prepares the key schedule for DES rounds.
  - `cpkey` and `usekey`: Manage the internal key register.

- **Encryption and Decryption**:
  - `des_enc`: Encrypts data in blocks of 8 bytes.
  - `des_dec`: Decrypts data in blocks of 8 bytes.
  - `des`: Encrypts or decrypts a single block of 8 bytes.

- **Helper Functions**:
  - `scrunch` and `unscrun`: Convert between byte arrays and 32-bit words.
  - `desfunc`: Core DES function that performs the 16 rounds of encryption or decryption.

- **Test Cases**:
  - `bruce_schneier_test`: Validates the implementation using known test vectors.
  - `custom_test_case`: Demonstrates encryption and decryption of a sample string.
 
## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- The DES implementation is based on the algorithm described in "Applied Cryptography" by Bruce Schneier.
- Special thanks to James Gillogly and Phil Karn for their contributions to DES key scheduling.
