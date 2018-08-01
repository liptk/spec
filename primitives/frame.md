# Frame

A frame is a container for any primitive (except itself), and each primitive has it's own unique frame ID.

## Parts

- The primitive's [FrameId](#frame-ids)
- The primitive itself

## Binary encoding

| length          | parameter  |
| --------------- | ---------- |
| 1 byte          | FrameId    |
| remaining bytes | primitive  |

## Frame Ids

| primitive                               | id     |
| --------------------------------------- | ------ |
| [Message](./message.md)                 | `0x01` |
| [Tag](./tag.md)                         | `0x??` |
| [Digest](./digest.md)                   | `0x??` |
| [Signature](./signature.md)             | `0x??` |
| [PublicKey](./keys/public-key.md)       | `0x??` |
| [SecretKey](./keys/secret-key.md)       | `0x??` |
| [SharedKey](./keys/shared-key.md)       | `0x??` |
| [DerivedKey](./keys/derived-key.md)     | `0x??` |
| [SealedBox](./boxes/sealed-box.md)      | `0x??` |
| [SignedBox](./boxes/signed-box.md)      | `0x??` |
| [TaggedBox](./boxes/tagged-box.md)      | `0x??` |