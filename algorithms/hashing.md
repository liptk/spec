# Hashing

## Algorithms

### `SHA256` (`0x01`)

#### Digest parameters

| length   | parameter    |
| -------- | ------------ |
| 32 bytes | digest bytes |

### `SHA512` (`0x02`)

#### Digest parameters

| length   | parameter    |
| -------- | ------------ |
| 64 bytes | digest bytes |

### `BLAKE2B` (`0x03`)

- Variable bit digests

#### Digest Parameters

| length     | parameter    |
| ---------- | ------------ |
| 1 byte     | digest-len   |
| digest-len | digest bytes |