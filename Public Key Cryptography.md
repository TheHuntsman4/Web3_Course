
### What is the chapter about?

The need to encrypt data and thus provide security is one of the most imprortant features of Web3. How do we acheive this? Well the idea discussed in this chapter is about how to use a technique called Public Key Encryption.

### What is Public Key Encryption?

In this type of encryption, there are two keys; a public key and a private key. The Public key as the name implies is shared with the public and is given to people with whom we wish to communicate with. Then there is the private key, which the original person retains. What this allows us to do is Authentication.
Only people with the public key can talk to us. So even if the data or messahe is intercepted by someone the whole thing would be useless as the message would be encrypted and it can only be read by the holder of the private key, which acts as the decryption provider.
There are many methods of employing this. The ones which we are gonna be using are called RSA and ECDSA.

## Problem statement

#### The first step in ECDSA is to hash the message before applying the signature algorithm. So if you wanted to sign a message with one your keypairs saying that you "Vote Yes on Proposal 327", the first step would be to hash this message: After we have the message hash we can sign it with our private key to prove that a particular address votes yes on proposal 327


### Hashing a message

In this exercise, we hash a message using ECDSA.
https://university.alchemy.com/course/ethereum/sc/631631e2d13b2d24e60dcceb/stage/63163222d13b2d24e60dccec

### Signing the message.

This is the next part of the process, telling the network that is it US who is authenticating this message or transaction. This is acheived by a process called signing.
https://university.alchemy.com/course/ethereum/sc/631631e2d13b2d24e60dcceb/stage/631697a65e3e3cb715cc63e4

### Retreiving the key from the recovery bit

When the signature is passed with all of its components (recovery bit included), the public key can be recovered. This means that blockchain nodes will be able to understand who signed the transaction that was sent to them. A transaction could indicate the user would like to send 1 ether to another address and provide a certain transaction fee. Since the signature signs the hash containing this intention, it is enough to authenticate this action entirely.

https://university.alchemy.com/course/ethereum/sc/631631e2d13b2d24e60dcceb/stage/6316a3f1505aa70c2106fbbe