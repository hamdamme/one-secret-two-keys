# Sources and further reading

These sources support the concepts in this guide. The guide's explanations and diagrams are original summaries; use the linked documents for precise definitions and requirements.

## Standards and security guidance

- [RFC 9180: Hybrid Public Key Encryption](https://www.rfc-editor.org/rfc/rfc9180) — defines a construction combining a KEM, KDF, and AEAD.
- [NIST glossary: Public-key cryptography](https://csrc.nist.gov/glossary/term/public_key_cryptography) — definitions and references for public-key cryptography.
- [NIST SP 800-56A Rev. 3](https://csrc.nist.gov/pubs/sp/800/56/a/r3/final) — recommendations for pair-wise key-establishment schemes. NIST has announced that it plans to update this publication, so check its page for newer guidance.
- [OWASP Cryptographic Storage Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html) — application-oriented guidance on encryption choices and key handling.

## How to read the sources

This repo is an introduction, not a replacement for a standard or security review. Standards define exact protocol behavior; implementation guidance depends on the software, threat model, and requirements.
