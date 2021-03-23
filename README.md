# Microsoft SEAL with CKKS-FV Transciphering

Microsoft SEAL is an easy-to-use open-source (MIT licensed) homomorphic encryption
library developed by the Cryptography and Privacy Research group at Microsoft.
For more details about SEAL and its installation guide,
see [SEAL_README.md](SEAL_README.md).

This forked repository adds a new scheme type named CKKS-FV to SEAL version 3.4.5.
It is built for implementation of CKKS-FV hybrid framework with the HERA cipher
proposed in
[Hybrid Framework for Approximate Computation over Encrypted Data](https://eprint.iacr.org/2020/1335).
In the CKKS-FV scheme, encoding/encryption and homomorphic evaluation are done in
FV style, and decryption/decoding are done in CKKS style. The CKKS-FV scheme also
offers conversion from FV ciphertexts to corresponding CKKS ciphertexts in the
lowest level. For more details, see [Changes.md](Changes.md).

