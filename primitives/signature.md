# Signature

A signature is the result of a signing algorithm on a message.

## Parts

- The [SigningAlgId](../algorithms/signing.md) used to produce the signature
- The [SignatureParams](../algorithms/signing.md) used for verification

## Binary encoding

| length                | parameter       |
| --------------------- | --------------- |
| 1 byte                | SigningAlgId    |
| `SignatureParams-len` | SignatureParams |