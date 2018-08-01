# Specification meta

## Primitives

- Primitives should be generic for their concept, and specify the concrete type and parameters inside.

For example, a `PublicKey` is a common concept in asymmetric cryptography, and can represent a signing, or key-exchange public part.

## Algorithm & Frame IDs

- Valid value is in the range `1..244` (`0` and `255` are reserved).
- `255` will be used for extending the range via a second byte, if ever there is a need (preferrably not). Library maintainers should just validate the range.

## Parameters

- Parameters should be encoded in minimal form.
- Parameters that need not change for the sake of security, or practical future proofing should be part of a unique algorithm ID.
- An algorithm must have a fixed set of parameters with a bounded size. 
- "Optional parameters" are either constant for the algorithm ID or explictly passed (while following the above points).

For example a `ED25519_SHA512` public-key:

- Encoded to a compressed edwards Y value (minimal form).
- The hash function (`SHA-512`) specifies the internal hashing algorithm (is a secure constant, and future proof).