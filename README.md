# Secure Chat Application

This is a Python-based chat application built as a college project. It enables two users to communicate over a network using socket programming while ensuring confidentiality and integrity of the transmitted data.

## Key Features

This project uses the AES (Advanced Encryption Standard) protocol for encrypting and decrypting messages, providing strong security against interception or tampering.

Messages are encrypted using AES in CBC (Cipher Block Chaining) mode, and a SHA-256 hashed passphrase is used as the symmetric key. An initialization vector (IV) is generated randomly for each message to further strengthen security.

The encryption key is derived from a passphrase to maintain secrecy, and padding is added to messages to ensure proper block size alignment. All encrypted messages are base64-encoded before transmission.

## How to Run
1. Install Python 3 on your system.
2. Install the pycryptodome library using: pip install pycryptodome
3. Open two terminal windows.
4. Run host.py in one terminal to start the server.
5. Run sever.py in the other terminal and enter the hostname shown by the server.
6. Begin secure chat between the two systems.

## Dependencies
Python 3
pycryptodome for AES encryption and random IV generation

### Disclaimer

This project is intended for educational use only and demonstrates basic principles of secure communication using symmetric encryption.
