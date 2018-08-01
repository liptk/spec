# Digest

A digest is the result of a hashing algorithm on a message.

## Parts

- The [HashAlgId](../algorithms/hashing.md) used to produce the digest
- The [DigestParams](../algorithms/hashing.md)

## Binary encoding

| length             | parameter    |
| ------------------ | ------------ |
| 1 byte             | HashAlgId    |
| `DigestParams-len` | DigestParams |