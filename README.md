# IShield: Encoder/Decoder Steganographic Model

An encoder/decoder system for protecting sensitive information by combining 
cryptography with audio steganography. Built as a final year project for 
B.Sc. Software Engineering at Topfaith University.

## Overview
IShield conceals encrypted messages inside WAV audio files using:
- **Enhanced Playfair Algorithm** — encrypts plaintext messages using a 10x9 
  matrix supporting uppercase/lowercase letters, numbers, and special characters
- **Two Least Significant Bit (2LSB) Encoding** — embeds the encrypted message 
  into the second-layer LSBs of audio samples, preserving audio quality

## Features
- Encode: hide encrypted text inside a WAV cover file
- Decode: extract and decrypt hidden text from a stego audio file
- Report: view and play previously generated stego files
- Login-protected access

## Tech Stack
Java (NetBeans IDE) for the GUI, Python for audio steganography and encryption logic.

## How It Works
1. User inputs a message and an encryption key (min. 8 characters)
2. Message is encrypted using the Enhanced Playfair Algorithm
3. Encrypted message is embedded into the 2nd LSB layer of a WAV file
4. Resulting stego file sounds identical to the original but carries hidden data
5. Decoding reverses the process to recover the original message

## Results
Successfully embedded and retrieved hidden information without noticeable 
audio distortion, demonstrating that combining encryption with steganography 
provides stronger protection than encryption alone.

## Author
Etini Akaninyene Unaam — B.Sc. Software Engineering, Topfaith University (2026)
Supervisor: Mr. Emmanuel Nyoho
