# KDF (Key Derivation Function)

## Algorithm IDs

| id     | algorithm             |
| ------ | --------------------- |
| `0x01` | [`PBKDF2`](#pbkdf2)   |

## Algorithms

### `PBKDF2`

#### Parameters

| length           | parameter  |
| ---------------- | ---------- |
| 4 bytes          | iterations |
| 2 bytes          | salt-len   |
| `salt-len` bytes | salt       |
