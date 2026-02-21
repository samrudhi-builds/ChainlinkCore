# Blockchain Demo

A simple blockchain implementation in JavaScript using linked list data structure. This project demonstrates the core concepts of blockchain technology including block creation, hashing, and chain linking.

## Features

- **Block Creation**: Each block contains an index, timestamp, data, previous hash, and its own hash
- **SHA-256 Hashing**: Cryptographic hashing ensures data integrity
- **Linked Chain Structure**: Blocks are linked together using a linked list implementation
- **Genesis Block**: Automatically creates the first block in the chain

## Installation

This project uses [Bun](https://bun.sh) - a fast all-in-one JavaScript runtime.

```bash
bun install
```

## Usage

Run the blockchain demo:

```bash
bun run index.js
```

Or use the npm script:

```bash
bun start
```

## How It Works

The blockchain consists of two main classes:

### Block Class
Each block contains:
- `index`: Position in the chain
- `timestamp`: When the block was created
- `data`: The actual data stored in the block
- `previousHash`: Hash of the previous block (ensures chain integrity)
- `hash`: SHA-256 hash of the current block's contents
- `next`: Reference to the next block in the chain

### Blockchain Class
Manages the chain with methods to:
- Create the genesis (first) block
- Add new blocks to the chain
- Print the entire chain

## Example Output

```
Block 0: [genesis hash]
Block 1: [block 1 hash]
Block 2: [block 2 hash]
```

## Requirements

- Bun runtime (v1.0+)

## License

MIT
