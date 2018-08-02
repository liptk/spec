# Hashing

## Algorithm IDs

| id     | algorithm             |
| ------ | --------------------- |
| `0x01` | [`SHA256`](#sha256)   |
| `0x02` | [`SHA512`](#sha512)   |
| `0x03` | [`BLAKE2B`](#blake2b) |

## Algorithms

### `SHA256`

#### Digest parameters

| length   | parameter    |
| -------- | ------------ |
| 32 bytes | digest bytes |

### `SHA512`

#### Digest parameters

| length   | parameter    |
| -------- | ------------ |
| 64 bytes | digest bytes |

### `BLAKE2B`

- Variable bit digests

#### Digest Parameters

| length     | parameter    |
| ---------- | ------------ |
| 1 byte     | digest-len   |
| digest-len | digest bytes |