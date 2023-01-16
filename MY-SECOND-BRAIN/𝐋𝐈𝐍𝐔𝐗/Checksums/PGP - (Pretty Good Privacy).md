- Pretty Good Privacy (PGP) is an [encryption program](https://en.wikipedia.org/wiki/Encryption_software) that provides [cryptographic](https://en.wikipedia.org/wiki/Cryptographic) [privacy](https://en.wikipedia.org/wiki/Privacy) and [authentication](https://en.wikipedia.org/wiki/Authentication) for [data communication](https://en.wikipedia.org/wiki/Data_communication).

- PGP is used for [signing](https://en.wikipedia.org/wiki/Digital_signature), encrypting, and decrypting texts, [e-mails](https://en.wikipedia.org/wiki/Email), files, directories, and whole disk partitions and to increase the [security](https://en.wikipedia.org/wiki/Security) of e-mail communications

![[250px-Public-key-crypto-1.svg.png|500]]

What is Public Key Cryptography?

- Through mathematical magic, you create a pair of keys (a keypair) consisting of a public key (pk) and a secret key (sk), sometimes called a private key

- You give people with whom you communicate (“friends”) a copy of your public key. You keep your secret key to yourself.

- (How you securely get a copy of your real public key to your friends is a topic all unto itself, but let’s just assume your friends have your real public key).

- Using a second bit of mathematical magic, a function encrypts a message using a public key such that encrypted message (ciphertext) can only be decrypted with the corresponding secret key. This is how you send a message:


> ENCRYPT (Message + Public key) = Ciphertext

and then you send the ciphertext over a communications channel.

Ciphertext = In cryptography, ciphertext or cyphertext is the result of encryption performed on plaintext using an algorithm, called a cipher

To reverse it, you run:

> DECRYPT (Cipertext + Secret Key) = Message

So, what is a signature?

- A signature nearly the opposite of encryption.

- You have a message that you want to make sure gets through without tampering, and is provably written by you.

- In the case of a signature, a message gets sent along with the output of a third bit of mathematical magic called a [cryptographic hash function](https://en.wikipedia.org/wiki/Cryptographic_hash_function) which produces a fixed-size “hash” sometimes called a “digest” or “checksum.”

- This “hash” of the message has an extremely high probability of being producible only by that very message.

For example : -

- the SHA-1 digest of “The quick brown fox jumped over the lazy dog” is F6513640F3045E9768B239785625CAA6A2588842.

- For all practical purposes, no other string of text will produce that digest.

- As a result, that digest can serve as a “signature” when sent along with that message to proves that the message was not tampered with.