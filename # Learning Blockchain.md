# Learning Blockchain (BC)

## Module 1: BC Intuition
### Fundamentals of BC
* BC is a continuously growing list of records, called blocks, which are linked and secured using cryptography.
* Blocks can contain 
	* data
	* previous hash
	* own hash
A digital hash is a fingerprint of some data. 

The first block of a blockchain is called the __Genesis block__. The prev.hash of a G-block is 000000. The OwnHash will have some value. 

Every subsequent block will have a prev hash (from the earlier block ) and its own hash. 

Its hard to tamper with a block, since its easy to see the broken link.

### Understanding SHA256 Hash
SHA256 is a core building block of BC. 
SHA = Secure Hash Algorithm - 256: Bits in memory.
It is 64 charcters
It is a hexadecimal hash, 

Invented by NSA. 

The code is open_source. 

There are other SHA algos. 
The 5 requirements of a Hashing Algo are:
1. One way 
2. Deterministic: The same document / data must generate the same hash
3. Fast computation
4. Avalance Effect: A small change (even 1 bit) to the data must comletely change the hash. 
5. Must withstand collisions: two pieces of data do not produce the same hash. While this happens, it must be extremely rare. Most importantly - must withstand artificial collisions. If a collision can be forged, then documents and contracts can be forged - this is bad. 


### Immutable Ledger
all transactions are stored on a ledger that are immutable - cannot be tampered with. 

### Distributed P2P Network
All new transactions are added on the chain. The networks are constantly checking their peers to see if the blockchains match up. 

### Mining Part1
Each block, apart from the data, and the prev Hash and current Hash also has one a field called Nonce
Nonce: Number used only once. 
This is the field used in mining. 


### Mining Part2
The Hash that identifies each block is a 64digit number that represents the SHA256 hash of a value. 

The Hash represents an actual number. Hashes that don't have all the 64 bits filled have leading 0s. 
The way mining works is that if you write a all the hashes in a hashing table. A target hash is identified, which will be the next hash in the sequence. 
	
Now, there is no way to know what number produces the target hash from the SHA-256 algorithm, because of the Avalanche effect. The only way to produce the hash is to run through a list of numbers (NONCEs) and see what hash comes through. 

So Bitcoin miners churn through hours of computing power, through several nonces to arrive at the target hash. Once they do, the bitcoin has become successful. 




The hash 
__Byzantine Fault Tolerance__
__Consensus Protocol Part1__
__Consensus Protocol Part2__
__BlockChain Demo__

### What is a BC
## Module 1: Create a BC
Walkthrough of how to program a BC

## Module 2a: CryptoCurrency(CC) Intuition
Fundamentals of how CC works

## Module2b: CC transactions
How transactions work.

## Practice modules 

## Module 3: Smart Contracts Intuition

## Module 3: Create a smart contract 
Imitate an ICO



