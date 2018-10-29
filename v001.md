# cooperative-consensus
inter-chain cooperative consensus protocol

Basic Concept

Using another (POW) blockchain’s block hash as the seed of random number generator. Using this random number to determine who will be the next block producer. 

To avoid manipulation of source block hash, we will use a certain type of slow sequential functions H that takes a long time to compute. the H(hash) is the random number.

Alternatively, we could use a certain type of hide-and-reveal scheme.  Where multiple people will hides a certain value and reveal it after the block is generated.  Then they will reveal the value.  The final random number would be becomes H(blockhash || a_private || b_private).

To avoid dependency on a single blockchain, the system can utilize several blockchains. The random number would be based on the hash from multiple blockchains.
