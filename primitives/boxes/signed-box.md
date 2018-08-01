# SignedBox

A signed box contains a message and it's associated signature.

## Parts

- The [Message](../message.md) that was signed
- The [Signature](../signature.md) produced from signing

## Binary encoding

| length                | parameter     |
| --------------------- | ------------- |
| 2 byte                | Signature-len |
| `Signature-len` bytes | Signature     |
| remaining bytes       | Message       |