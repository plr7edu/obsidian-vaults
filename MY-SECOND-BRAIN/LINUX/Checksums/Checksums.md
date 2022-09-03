## Verify Signature (Checksums)
- It is recommended to verify the image signature before use, especially when downloading from an HTTP mirror, where downloads are generally prone to be intercepted to [serve malicious images](https://www2.cs.arizona.edu/stork/packagemanagersecurity/attacks-on-package-managers.html).

![[hexadecimal-code-security-key-krzysztof-zmij-e-plus-getty-images-57c76b825f9b5829f4bd185e.jpg |400]]

## Checksums Explained

- A checksum is a value that represents the number of [bits](https://whatis.techtarget.com/definition/bit-binary-digit) in a transmission message and is used by [IT](https://searchdatacenter.techtarget.com/definition/IT) professionals to detect high-level errors within data transmissions.

- Prior to transmission, every piece of data or file can be assigned a checksum value after running a cryptographic hash function.

- Checksums work by giving the party on the receiving end information about the transmission to make sure that the full range of data is fully delivered.

- The checksum value itself is typically a long string of letters and numbers that act as a sort of fingerprint for a file or set of files to indicate the number of bits included in the transmission.

- If the checksum value calculated by the end user is even slightly different from the original checksum value of the file, it can alert all parties in the transmission that the file was corrupted or tampered with by a third party.

- From there, the receiver can investigate what went wrong or try re-downloading the file.

![[330px-Checksum.svg.png]]
- By themselves, checksums are often used to verify data integrity but are not relied upon to verify data [authenticity](https://en.wikipedia.org/wiki/Authentication).

- A checksum is also sometimes called a ==hash sum== and less often a ==hash value,== hash code, or simply a hash , checksum function or [checksum algorithm](https://en.wikipedia.org/wiki/Checksum_algorithm).

- To produce a checksum, you run a program that puts that file through an [algorithm](https://www.howtogeek.com/howto/44052/htg-explains-what-are-computer-algorithms-and-how-do-they-work/).

- Typical algorithms used for this include ==MD5, SHA-1, SHA-256, and SHA-512.


## Common types of checksum algorithms

- There are multiple cryptographic hash functions that programmers can use to generate checksum values.

A few common ones include :- 

#### **SHA-0 : - 

- This hash function was the first of its kind and it was withdrawn shortly after its creation in 1993.

#### **SHA-1 : -

- This hash function was no longer considered secure as of 2010.

#### **SHA-2 (224, 256, 384, 512)  : – 

- This family of hash functions relies on sounds and numbers to create a checksum value.
- The resultant checksums are vulnerable to length extension attacks, which involve a hacker reconstructing the  internal state of a file by learning its hash digest.

#### MD5 :-

This hash function creates a checksum value, but each file will not necessarily have a unique number, so it is open to vulnerabilities if a  hacker swaps out a file with the same checksum value.

### Comparison Chart (MD5 VS SHA-1)

![[Difference-between-MD5-and-SHA-1.png]]


| Basic Terms                   | MD5                                                                | SHA-1                                                                                              |
| ----------------------------- | ------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------- |
| Meaning                       | Commonly<br> used hash algorithm for producing 128-bit hash value. | It is a set of cryptographic hash functions for producing 264 – to<br> 2128 –<br> bits hash value. |
| Discovered By             | Ron<br> Rivest                                                     | U.S.<br> National Institute of Standards and Technology                                            |
| Long<br> Form                 | Message-Digest<br> Algorithm                                       | Secure<br> Hash Algorithm                                                                          |
| Security                      | Less<br> secured                                                   | More<br> secured                                                                                   |
| Speed                         | Faster                                                             | Less<br> fast                                                                                      |
| Attacks                       | Prone<br> to attacks                                               | Less<br> prone to attacks                                                                          |
| Buffer<br> space              | 128<br> bits                                                       | 160<br> bits                                                                                       |
| Year<br> of publishing        | 1992                                                               | 1995                                                                                               |
| Uses                          | little-endian<br> scheme                                           | big-endian<br> scheme                                                                              |
| Iteration<br> Number          | 64                                                                 | 80                                                                                                 |
| Rounds                        | 16                                                                 | 20                                                                                                 |
| Simplicity<br> and complexity | Simple                                                             | Complex                                                                                            |


### Links 
1. [[MD5  (Message-Digest Algorithm)]]
2. [[SHA - 1 (Secure Hash Algorithm)]]
3. [[PGP - (Pretty Good Privacy)]]