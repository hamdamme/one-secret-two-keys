# One Secret, Two Keys

A short visual guide to two common cryptographic key models:

- **Shared-key cryptography:** both sides use the same secret key.
- **Public-key cryptography:** a related public/private key pair supports specific tasks such as key agreement, encryption, or signatures.

The main idea: these approaches often work together. Public-key techniques can help two parties establish key material; symmetric authenticated encryption can then protect the actual message.

## Start here

1. [Shared keys](guides/shared-keys.md)
2. [Public and private keys](guides/public-and-private-keys.md)
3. [How they work together](guides/how-they-work-together.md)
4. [Sources](sources.md)

## What makes this guide different

This is a small concept guide, not a catalog of every cipher or library. It uses diagrams and plain-language comparisons to explain how the key types relate. Examples are educational and are not production-ready implementations.

## Scope

This guide explains concepts. It does not recommend designing a custom cryptographic system. For real software, use established protocols and maintained cryptographic libraries, and get security review appropriate to the application.
