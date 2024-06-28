For this project, I developed two functions for encryption and decryption using
XOR operation with a shared key. I used the QKD distribution BB84 protocol
to generate a shared key. The encryption function takes the shared key and
message as arguments and returns the encrypted message. Similarly, the de-
cryption function takes the encrypted message and shared key as inputs and
returns the original message.


The function iterates through each character in the message and it pairs it
with the corresponding bit in the key. Using the binary value (ASCII value
changed into binary) of each character I operate the XOR operation. Finally
encryption function changes it back to character as an encrypted message. A
similar process repeats in the decryption function for encrypted messages.
One of the problems I encountered was the shared key didn’t have a good
mix of 1 and 0. So, a biased key could weaken the encryption more susceptible
to attacks. Also, in my project, I realized that as my message gets longer the
shared key should also increase proportionally. So number of qubits shared
should be equal if not larger than the message length. This problem might be
solved using some techniques of increasing the length of the present shared key.
