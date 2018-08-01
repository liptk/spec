# DerivedKey

A derived key is the result of a KDF algorithm over some data.

## Parts

- The [KdfAlgId](../algorithms/kdf.md) used to produce the DerivedKey
- The [KdfAlgParams](../algorithms/kdf.md) used

## Binary encoding

| type                     | parameter         |
| ------------------------ | ----------------- |
| 1 byte                   | KdfAlgId          |
| 2 bytes                  | KdfAlgParams-len  |
| `KdfAlgParams-len` bytes | KdfAlgParams      |
| remaining bytes          | derived-key bytes |