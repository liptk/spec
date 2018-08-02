# TaggedBox

A tagged box contains a message and it's associated tag.

## Parts

- The [Message](../message.md) that was tagged
- The [Tag](../tag.md) produced from a MAC algorithm

## Binary encoding

| length          | parameter |
| --------------- | --------- |
| 2 byte          | Tag-len   |
| `Tag-len` bytes | Tag       |
| remaining bytes | Message   |