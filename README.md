# Running Platform

The python project was tested to run on Google Colab but should run on any notebook-type IDE such as Jupyter Notebook

# Initialization

Start by running the first code block on the project, labelled under "Setup" to install the required libraries for the QRNG and the cryptography use-case sample

# QRNG

The quantum circuit is of 128 qubits, that is done through a loop as the limitation of the used quantum computer simulation backend is 29 qubits, and each qubit is simply connected to a Hadamard gate that is measured right after to get the random value of 0 or 1 for each normal bit.

# AES Encryption and Decryption use-case

The output from the QRNG is then formatted into the form needed by the encryption library used (pycryptodome) and then plugged into the AES encryption algorithm as the key. This code blocks has the outputs of the encrypted message as well as the message after the decryptions, which would realistically be on the receiving end of a data transmission or the hash of a password in a database.