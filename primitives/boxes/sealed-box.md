# SealedBox

A sealed box contains an encrypted message.

## Parts

- The [AeadAlgId](../../algorithms/aead.md) used
- The [AeadAlgParams](../../algorithms/aead.md)
- The encrypted [Message](../message.md)

## Binary encoding

| length                    | parameter          |
| ------------------------- | ------------------ |
| 1 byte                    | AeadAlgId          |
| `AeadAlgParams-len` bytes | AeadAlgParams      |
| remaining bytes           | encrypted(Message) |