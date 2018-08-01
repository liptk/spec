# Tag

A Tag is the result of a MAC algorithm on a message.

## Parts

- The [MacAlgId](../algorithms/mac.md) used to produce the tag
- The [TagParams](../algorithms/mac.md)

## Binary encoding

| length        | parameter |
| ------------- | --------- |
| 1 byte        | MacAlgId  |
| TagParams-len | TagParams |