# AEAD (Authenticated Encryption)

## Algorithms

### `XCHACHA20_POLY1305` (`0x01`)

- TODO, find good spec.
- Requires a 256 bit key.
- Produces 512 bit blocks and a 128 bit mac tag.

#### Parameters

| length   | parameter |
| -------- | --------- |
| 24 bytes | nonce     |

### `CHACHA20_POLY1305` (`0x02`)

- As per [ITEF RFC7539](https://tools.ietf.org/html/rfc7539).
- Requires a 256 bit key.
- Produces 512 bit blocks and a 128 bit mac tag.

#### Parameters

| length   | parameter |
| -------- | --------- |
| 12 bytes | nonce     |

### `AES_256_GCM` (`0x03`)

- As per [ITEF RFC5116](https://tools.ietf.org/html/rfc5116).
- Requires a 256 bit key.
- Produces 128 bit blocks and a 128 bit mac tag.

#### Parameters

| length   | parameter |
| -------- | --------- |
| 12 bytes | nonce     |

## Binary encoding

Just the nonce bytes on their own.