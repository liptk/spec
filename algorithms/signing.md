# Signing

## Algorithm IDs

| id     | algorithm                           |
| ------ | ----------------------------------- |
| `0x01` | [`ED25519_SHA512`](#ed25519_sha512) |

## Algorithms

### `ED25519_SHA512`

#### Signature Parameters

As per ED25519 specification.

| length   | parameter |
| -------- | --------- |
| 32 bytes | `R` bytes |
| 32 bytes | `S` bytes |