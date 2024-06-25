## Encryption
> Encryption is the act of taking readable text
and scrambling it so it can only be read by a recipient that has the decryption key.

Plaintext: Data that has not been encrypted

Cipher: Algorithms used to scramble plain text

CipherText: Encrypted plain text

> The person on the receiving end has a decryption key that's used to decrypt (or unscramble) the data so it's in a readable or useable format.

Some industries require data encryption:
* Student records, health records, consumer data
* Many OSes also have built-in encryption

## Data at rest
> Data at rest refers to data that resides on a storage device. The files aren't open or being transmitted anywhere.

Can be encrypted at:
* File level
* Storage device level (disks & drives)
    * Software-based encryption
    * hardware-based encryption (Bit locker)
* Cloud level

DAR is less vulnerable `but not immune` from attacks

> Using updated firewalls, VPNs, and anti-malware helps keep your data safe.

## Data in motion
> data that is actively moving between two devices

Eg: two computers, mobile device and mail server, computer and bank's online website

All HTTPs websites are encrypted:
* but hackers can compromise encrypted sites with social engineering, man-in-the-middle attacks and password cracking 
* They can also create `their own encrypted HTTPs sites` that install malware

> DIM is especially at risk to intervention like M-I-T-M so we need to use `e2e encryption` so that hacker cannot decrypt the data even if they get it 

VPN networks are encrypted but `not always e2e`

## Symmetric Encryption (Single Key/Private key)
*  Single key is used between parties to encrypt and decrypt data.

With only one key, symmetric encryption:
* Uses less memory - great for quickly and securely processing large amounts of data
* Often used as a `session key` because it is difficult to keep a single key secret 
* Symmetric encryption technologies: 3DES and CAST

## Asymmetric Encryption (Private & Public key)
* Aka public key cryptography uses a public key and private key
* More complex and used for `smaller amounts of data`
* Safe to share the public key for encryption or decryption because only private key can undo the public key's action
* Uses include:
    1. Authentication
    2. Digital Certificates
    3. Digital Signatures
    4. Key Exchange - symmetric encryption key is shared only to intended recipients

RSA (Rivest-Shamir-Adleman) is mainly used for asymmetric encryption 

## Public Key Infrastructure (PKI)
> When a user is validated with a digital certificate by a Certificate Authority (CA).

How it works:
1. The digital certificate has a public encryption key that encrypts data.
2. If the data recipient trusts the CA that issued the digital certificate, they use a private key to decrypt the data.

Use case: Smart Card Authentication
1. Smart card has public/private key pair
2. It presents a digital certificate (including public key) to the server its trying to access
3. If the server trusts the CA that issued the digital certificate, it will use the public key to send an encrypted request.
4. Only the smart card’s private key can decrypt the request, which means only the smart card owner can send the correct response.

> Slightly different for digital signature
1. The sender sends an encrypted signature and a public decryption key to a recipien
2. If the recipient can decrypt the signature with the public key, that proves the sender signed it because they must have `performed` the encryption with the `private key`  (Non-repudiation) - cannot deny that they signed


## Cryptographic Hashes
> A cryptographic hash is a short string of numbers and letters created by running a password or file through an algorithm.

> A single password and a full library will have different cryptographic hashes,
but each will have the same number of characters.

If any data is altered or removed from pw or file:
* Cryptographic hash will be different
* Any difference in cryptographic hash will let the system know that the data has been tampered with
* This is how it works in password systems, they store the c-hash of ur first password and see if it matches with the c-hash of the password u type on ur next login

> C-hashes save space, authenticate data and keeps information secure
