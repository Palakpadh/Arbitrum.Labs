# Arbitrum.Labs
An interactive Proof-of-Work (PoW) simulator for blockchain consensus. It uses the browser's Web Crypto API to calculate real-time **SHA-256 hashes** by linking a block’s data, nonce, and the previous block's hash.  Mining increments the nonce until a `"00"` prefix is found. Altering Block 1 breaks the chain, illustrating blockchain immutability.
