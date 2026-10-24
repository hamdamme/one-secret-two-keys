# Public and private keys

Public-key cryptography uses a related pair: a **public key** that can be shared, and a **private key** that its owner must protect. The pair is made for particular cryptographic operations; not every key pair can be used for every operation.

## Three different jobs

### 1. Encryption to a recipient

A sender uses the recipient's public key in a scheme designed for encryption. The matching private key is needed to recover the protected message or key material.

```text
Sender: recipient's public key + message  → protected output
Recipient: matching private key + output → message
```

### 2. Key agreement

Two participants use their own private key and the other participant's public information to derive matching secret material. They do not send that secret itself across the network. The protocol must also address who the other party is; otherwise an attacker may substitute their own keys.

```text
Alice's private key + Bob's public information ─┐
                                                ├─→ matching secret material
Bob's private key + Alice's public information ─┘
```

### 3. Digital signatures

The signer uses a private signing key to create a signature. Others use the corresponding public verification key to check it. A signature can help establish who signed the data and whether it changed. It does **not** hide the data.

## Do not mix these up

- A public key is not a password and is not automatically proof of identity. It must be associated with the right person or service.
- Encryption and signatures solve different problems.
- Key agreement produces shared secret material; by itself it does not guarantee that the other participant is the person you intended.
