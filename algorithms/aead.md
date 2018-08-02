# AEAD (Authenticated Encryption)

## Algorithm IDs

| id     | algorithm                                   |
| ------ | ------------------------------------------- |
| `0x01` | [`XCHACHA20_POLY1305`](#xchacha20_poly1305) |
| `0x02` | [`CHACHA20_POLY1305`](#chacha20_poly1305)   |
| `0x03` | [`AES_256_GCM`](#aes_256_gcm)               |

## Algorithms

### `XCHACHA20_POLY1305`

- TODO, find good spec.
- Requires a 256 bit key.
- Produces 512 bit blocks and a 128 bit mac tag.

#### Parameters

| length   | parameter |
| -------- | --------- |
| 24 bytes | nonce     |

### `CHACHA20_POLY1305`

- As per [ITEF RFC7539](https://tools.ietf.org/html/rfc7539).
- Requires a 256 bit key.
- Produces 512 bit blocks and a 128 bit mac tag.

#### Parameters

| length   | parameter |
| -------- | --------- |
| 12 bytes | nonce     |

### `AES_256_GCM`

- As per [ITEF RFC5116](https://tools.ietf.org/html/rfc5116).
- Requires a 256 bit key.
- Produces 128 bit blocks and a 128 bit mac tag.

#### Parameters

| length   | parameter |
| -------- | --------- |
| 12 bytes | nonce     |