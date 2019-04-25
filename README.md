# Week 1

Bitcoin is decentralized, peer to peer (P2P), permission-less (no identity, open environment whereas permissioned model is closed and has identities) cryptocurrency.

### Bitcoin Block
Size 1 - 8 mb, has 
1. Block Header
   * Previous Block Hash 
   * Mining statistics used to construct the block (Bitcoin Mining: $H_k = Hash (H_{k - 1} | T | Nonce)$, "T" is the set of transactions, Nonce is such that $H_k$ has certain predefined complexity (i.e. number of zeros at the prefix). So the header as well contains current block's hash), so the header contains mining statistics such as timestamp, nonce and difficulty (difficulty determines the toughness of tampering with a block in blockchain) 
   * Merkle tree root (leaf contains hash of its item, interior node contains hash of its children thus its difficult to modify the tree, i.e. tamper proof)
2. List of transactions

### Applications
Smart Contracts, KickStarter (Crowd Funding)

### Side Info
* PoW - ensures consensus over a permision less setting based on challenge response.
* Transactions are psuedo anonymous, i.e., Transactions are sent to public key addresses (cryptographically generated addresses computed by wallet applications). We encrypt the transaction by the public key of the target address and only the target node can decrypt and accept the transaction.
* See supporting photos.
### Cryptographic Hashing
* X - Message, H(X) - Message digest
* A small change in data results in significant change in the output, known as Avalanche effect (consequently it helps in **hiding** the original message)
* If two messages are different then their digest also differs (**Collision-Free**)
	* Hash functions are one way, given x it is easy to find H(x) however given a H(x) no deterministic algorithm can find x.
	* It is difficult to find x, y such that x != y but H(x) = H(y). So to check whether x = y, we usually check whether H(x) = H(y) as digest is comparitively smaller.
* **Puzzle-Friendly** - Given X, Y find out k such that Y = H(X || k). Puzzle friendly property implies that random searching is the best strategy to solve the above puzzle.
* SHA256 (Secure Hash Algorithm that generates 256 message digest) is used in Bitcoin mining. See supporting photos. 

### Uselss
<details><summary>Click Me</summary>
<p>
Every peer maintains a local copy of the block chain, Requirements:
1. All the replicas need to be updated with the last mined block
2. All the replicas need to be consistent (copies need to be exactly similar)
</p>
</details>

# Week 2
Just see photos.

# Week 3
See slides and photos in the folder.

# Week 4, 5, 6, 7
See slides. Ignored lots of things in week 7.
Everledger - tracks provenance (the place of origin or earliest known history of something) of diamonds from mines to jewellery stores. 
we.trade - bc based international trading system for a consortium of major world banks.
(In HL Fabric) Only member with "Operator" permission can change the configuration of the channel. And we just have 3 permissions, viz., Reader, Writer and Operator.
Just have a look at assignment 7 answers.