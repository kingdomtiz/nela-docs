# Decentralized File Security

### ESeal

**The encryption structure of files is the core building block for enforcing security on files. Each file which is uploaded to Nela follows the following scheme:**

**Body -** The actual file is encrypted through symmetric encryption and a random key.

**Header -** The encrypted file contains with it a header, in which each identity's permissions as well as the body's random key are encrypted together using asymmetric encryption.

![EDFS file encryption protocol](.gitbook/assets/image.png)

​Authority and permissions can be to the degree of what can be done with the file (view, edit, create a duplicate, etc.) to what Operating System is accepted or if a hardware device is required.Through this encryption scheme, permissions on files can be given by only having knowledge of a user's public key, setting the foundation of trust-less access control management within Nela's encrypted decentralized file system.

### Real-Time Encryption/Decryption

Nela's approach to file security&#x20;

### Security Modules

#### DSFS & Security Sandbox

#### Local Service
