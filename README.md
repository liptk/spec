<p align="center">
    <img width="100" src="./logo.svg" alt="LIPTK" />
    <br />
    <strong>Lightweight tools for the cryptic!</strong>
</p>

<h3 align="center">NOTE THIS SPECIFICATION IS UNDER DEVELOPMENT!</h3>

LIPTK goal's are to provide a opinionated, yet flexible specification for providing cryptographic primitives (ie. cleartext, ciphertext, signatures, etc) with a way to encode and decode them safely.

## Why LIPTK?

**LIPTK** specifies sane defaults for algorithms and their parameters, and is designed so they can be composed seamlessly together. To do this, **LIPTK** provides generic primitives with concrete types and a format for encoding them to binary (and back).

This specification is inspired by `libsodium` as it specifies a small suite of algorithms that have been vetted quite extensively, however **LIPTK** strives to be more flexible in respect to providing more alternative algorithms, and a future proof way of using them. Implementations of this specification may actually use `libsodium` internally to provide support for algorithms.

You can also draw parallels between **LIPTK** and the **OpenPGP message format**, but **LIPTK**'s binary format is designed to provide the bare minimum, and is lightweight in comparison. You could build a protocol using **LIPTK** primitives similar to **OpenPGP** (which this library wants you to be able to do), but a higher level protocol is not in the scope of this project.

### Composable binary format

Rather than defining a strict specification on how you should talk, **LIPTK** provides you primitives you can use to compose your own conversation easily.
For example, a format for encoding `ed25519` signature parameters is provided, and can be wrapped in a generic signature, which in turn can be passed over the network, without worrying how to externally specify what sort of signature it is. A **LIPTK** decoder implementation can then unwrap the signature to get it's parameters to verify data.