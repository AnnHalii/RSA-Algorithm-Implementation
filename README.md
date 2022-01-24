# RSA-Algorithm-Implementation

Course: Security of Infocommunication Networks (Zolotarev V.A.)
=============


RSA algorithm
=============

- Take two distinct, large primes `p` and `q`.
- Ideally these have a similar byte-length.
- Multiply `p` and `q` and store the result in `n`.
- Find the totient for `n` using the formula: ` 𝜑(𝑛) = (𝑝−1)⋅(𝑞−1) `.
- Take an `e` coprime that is greater, than 1 and less than `n`.
- Find `d` using the formula ` 𝑑⋅𝑒 ≡ 1 mod 𝜑(𝑛) `.
- At this point, the pair (`e`, `n`) is the public key and the private key (`d`, `n`) is the private key.

Features
--------

- Create a private and public keys.
- Messages Encryption 
- Messages Decrypted 

How to use
--------

- `git clone git@github.com:AnnHalii/RSA-Algorithm-Implementation.git`
- Run script `rsa.py`
- Example for `p` and `q` (prime numbers) you can find in file `primes.txt`
- Remember that `p` and `q` should not be small (the current standard for the \
internet is 128 bit encryption)