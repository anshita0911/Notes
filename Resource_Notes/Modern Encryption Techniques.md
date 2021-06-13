# Modern Encryption Techniques:

Modern encryption is the key to advanced computer and communication security. This stream of cryptography is completely based on the ideas of mathematics such as number theory and computational complexity theory, as well as concepts of probability. In this chapter, you will learn about the different elements and characteristics of modern cryptography.

## Types of Modern Cryptography

Different algorithms have come up with powerful encryption mechanisms incorporated in them. It gave rise to two new ways of encryption mechanism for data security. These are:

- Symmetric key encryption
- Asymmetric key encryption

**Key:** It can be a number, word, phrase, or any code that will be used for encrypting and decrypting any ciphertext information to plain text and vice versa.

Symmetric and asymmetric key cryptography is based on the number of keys and the way these keys work. Let us know about both of them in details:

### **Symmetric Key Encryption**

Symmetric key encryption technique uses a straight forward method of encryption. Hence, this is the simpler among these two practices. In the case of symmetric key encryption, the encryption is done through only one secret key, which is known as "Symmetric Key", and this key remains to both the parties. The same key is implemented for both encodings as well as decoding the information. So the key is used first by the sender prior to sending the message, and on the receiver side, that key is used to decipher the encoded message.

One of the good old examples of this encryption technique is Caesar's Cipher. Modern examples and algorithms that use the concept of symmetric key encryption are RC4, QUAD, AES, DES, Blowfish, 3DES, etc.

### **Asymmetric Key Encryption**

Asymmetric Encryption is another encryption method that uses two keys: a new and sophisticated encryption technique. This is because it integrates two cryptographic keys for implementing data security. These keys are termed as Public Key and Private Key. The "public key", as the name implies, is accessible to all who want to send an encrypted message. The other is the "private key" that is kept secure by the owner of that public key or the one who is encrypting.

Encryption of information is done through a public key first, with the help of a particular algorithm. Then the private key, which the receiver possesses, will use to decrypt that encrypted information. The same algorithm will be used in both encodings as well as decoding. Examples of asymmetric key encryption algorithms are Diffie-Hellman and RSA algorithm.

#### Security Provided by These Cryptography Algorithms

- Confidentiality of information.
- Data Integrity.
- Authentication.
  - Message authentication.
  - Entity authentication.
- Non-repudiation.

#### Techniques Work in Combination With Modern Cryptography

- Encryption and it's key
- Hash functions
- Message Authentication Codes (MAC)
- Digital Signatures

- Digital Signatures

#### Advantages and Characteristic Differences Between Classical/Traditional Encryption and Modern Encryption 

Here are the marked differences between the classical as well as the modern encryption techniques:

| Traditional Encryption                                       | Modern Encryption                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| For making ciphertext, manipulation is done in the characters of the plain text. | For making ciphertext, operations are performed on binary bit sequence. |
| The whole of the ecosystem is required to communicate confidentially. | Here, only the parties who want to execute secure communication possess the secret key. |
| These are weaker as compared to modern encryption.           | The encryption algorithm formed by this encryption technique is stronger as compared to traditional encryption algorithms. |

### Cryptographical Hash Function:

# What are cryptographic hash functions?

*What are cryptographic hash functions? Here are some variations that can improve your cryptographic hashes and provide a stronger barrier against attacks.*

A [cryptographic hash function](https://en.wikipedia.org/wiki/Cryptographic_hash_function) is an algorithm that takes an arbitrary amount of data input—a credential—and produces a fixed-size output of enciphered text called a hash value, or just “hash.” That enciphered text can then be stored instead of the password itself, and later used to verify the user.

Certain properties of cryptographic hash functions impact the security of password storage.

- **Non-reversibility, or one-way function.** A good hash should make it very hard to reconstruct the original password from the output or hash.
- **Diffusion, or avalanche effect**. A change in just one bit of the original password should result in change to half the bits of its hash. In other words, when a password is changed slightly, the output of enciphered text should change significantly and unpredictably.
- **Determinism.** A given password must always generate the same hash value or enciphered text.
- **Collision resistance.** It should be hard to find two different passwords that hash to the same enciphered text.
- **Non-predictable.** The hash value should not be predictable from the password.

## The good

Cryptographic hashes take cleartext passwords and turn them into enciphered text for storage. Attackers who access your database are forced to decipher those hash values if they want to exploit them. In other words, hashes slow down attackers.

## The bad

Simple cryptographic hashes can slow down attackers, but ultimately attackers will be able to overcome them.

- Attackers equipped with fast hardware can easily “crack” hashed credentials.
- Good hash algorithms are designed to be collision-resistant, but collisions are impossible to eliminate completely. MD5 and SHA-1 have been proven to contain known collisions—that is, produce the same hash value from different credentials.
- Rainbow tables are “optimized lookup tables” that can be used to reverse-engineer one-way hash functions. A rainbow table is basically a pre-computed set of plaintext strings and their corresponding hashes. Large rainbow tables are publicly available, and attackers can use one of these tables to retrieve cleartext data that has been hashed.

## Power up your cryptographic hashes

There are variations that can improve your hash function and provide a greater barrier against attacks.

### Salted hashes

[Salting](https://en.wikipedia.org/wiki/Salt_(cryptography)) adds random data to each plaintext credential. The result: two identical plaintext passwords are now differentiated in enciphered text form so that duplicates cannot be detected.

### Keyed hash functions

A keyed hash function (also known as a hash message authentication code, or HMAC) is an algorithm that uses a cryptographic key AND a cryptographic hash function to produce a message authentication code that is keyed and hashed.

### Adaptive hash functions

An adaptive one-way function is any function that is designed to iterate on its inner workings, feeding the output back as input, in a manner that causes it to–ultimately–take longer to execute. It is adaptive because the developer can adjust how many iterations occur. To protect stored passwords, architects have applied the adaptive design to hash functions (such as PBKDF2) and to encryption schemes (such as [bcrypt](http://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)).

## The trade-off of cryptographic hash functions

Cryptographic hash functions do provide barriers to attackers, like speed bumps slowing down a speeding motorcycle. But it’s critical to remember that eventually the motorcycle will still make it down the street. However, these barriers will slow down your defenders as well—normal users and your server. Set the speed bump too high, and you run the risk of annoying your user—and overtaxing your server.

But no matter how high you build your speed bump, an attacker WILL ultimately be able to overcome it. The ongoing challenge is to slow down attackers while balancing the needs and satisfaction of your users.

Examples:

#### Hash functions

- [MD5](https://en.wikipedia.org/wiki/MD5) - Widely used hash function producing a 128-bit hash value. MD5 was initially designed to be used as a cryptographic hash function, but it has been found to suffer from extensive vulnerabilities. It can still be used as a checksum to verify data integrity, but only against unintentional corruption.
- [SHA1](https://en.wikipedia.org/wiki/SHA-1) - Cryptographic hash function designed by the NSA. SHA-1 produces a 160-bit hash value known as a message digest. SHA-1 is no longer considered secure against well-funded opponents.
- [SHA2](https://en.wikipedia.org/wiki/SHA-2) - Set of hash functions designed by the NSA. SHA-256 and SHA-512 are novel hash functions computed with 32-bit and 64-bit words, respectively. They use different shift amounts and additive constants, but their structures are otherwise virtually identical, differing only in the number of rounds.

**Site:** [CyberChef](http://icyberchef.com/)

