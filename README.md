# Message-Integrity-verification
Description:
This Python application simulates a core cryptographic mechanism used to ensure data integrity across insecure channels. Built with tkinter, it allows two parties (Sender and Receiver) to verify that a message has not been tampered with during simulated transit using the SHA-256 hash algorithm.
This project is highly relevant to Distributed System Security and is a foundational demonstration of cryptographic trust.

Key Concepts Demonstrated:
•	Cryptographic Primitives: Practical implementation of the SHA-256 secure hash function using Python's hashlib.
•	Data Integrity & Non-Repudiation: Proving the ability to detect even a single-byte alteration in transmitted data.
•	Distributed Trust Model: Simulating the independent verification process used in digital signatures and blockchain technology.
•	GUI Development (UI/UX): Utilizing the tkinter library to wrap complex logic in an intuitive, user-friendly interface.

Usage and Testing:
The application is split into three steps to simulate the communication process:
1.	Sender Action: Enter an original message (e.g., "The secure meeting is tomorrow at 9 AM.") and click "Calculate Sender Hash." This hash represents the "digital fingerprint" sent alongside the message.
2.	Simulated Transit: The message is assumed to be sent.
3.	Receiver Verification:
o	Case 1 (Success): Copy the original message and paste it exactly into the "Message Received" field. Click "VERIFY MESSAGE INTEGRITY." The result will show VERIFIED.
o	Case 2 (Tampering Detected): Re-run the simulation. After calculating the Sender Hash, enter the original message into the "Message Received" field, but change one letter (e.g., change "9 AM" to "10 AM"). Click "VERIFY MESSAGE INTEGRITY." The result will show COMPROMISED due to the hash mismatch.

Output:

<img width="940" height="1021" alt="image" src="https://github.com/user-attachments/assets/3f0f6b79-fb60-4242-bc64-b1f757cc8289" />
<img width="940" height="838" alt="image" src="https://github.com/user-attachments/assets/64713b3d-9eec-4f29-9b1f-c5557ebbdb0f" />
