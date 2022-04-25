# The Nela Network

Nela Storage solution is divided into 2 working parts:&#x20;

1. a state-of-the-art KAD-based decentralized storage solution
2. 2\. Decentralized Content Acceleration Network (DSCAN)

All files on the decentralized storage are encrypted and secured, and users never interact directly with the decentralized storage as all access is governed by DSCAN via standard HTTP.&#x20;

this unique architecture allows for simple access from any device, and high performance due to caching of files, optimized routing, and fast retrieval of files

**Security**&#x20;

In Nela, we have a different approach to file security, as files are encrypted, and access permission is governed by the security modules. access to the encrypted file itself means very little, thus trustless access to any file on the network is simple and straightforward. No paywalls, passwords, or 2FA are ever needed.

**Access Control**&#x20;

Smart contracts are the interface to all access control operations. This provides many advantages, for one, every operation is journaled on-chain and therefore transparent. In addition, smart contracts can be automated, and are trustless by nature. A user can define conditions for file access, and set a price on the level of access (purchase, limited use, rental, and so forth.

**Programmable licensing** **on assets**&#x20;

The combination of security with the flexibility of smart contracts brings about the notion of programmable licensing, a file owner can program sophisticated and automatic licensing and use-right models directly into the network. This has far-reaching implications for many real-world business models. From licensing music, and videos to gaming, and in fact, any business, or individual who sells or rents access to documents, online files, or datasets.\
\
**Nela decentralized storage**

Nela decentralized storage is a state-of-the-art KAD network optimized for efficient scalability and encrypted file sharing and distribution. Nela decentralized storage has the following properties: \
\
1\. All stored files are encrypted A Simplified distributed hash table (DHT). \
2\. The Nela ESeal header and encrypted body are split into two different files. \
3\. File header is appendable. \


**A Simplified distributed hash table (DHT)**\
****In Nela decentralized storage, the DHT stores the hash index of the file rather than the hashes for the parts. Therefore, storage nodes in the network store information on file parts. When a node is searched, it returns the parts information that it contains. Thus, the DHT needs to be searched only once when downloading a file from the decentralized storage, resulting in increased efficiency.

**ESeal header** \
In many use cases, the ESeal file may be of significant size (for example, it may reach 100MB if a million people were to rent independently). Therefore, Nela decentralized storage supports using key-value to store each ESeal item in the ESeal header. Additionally, to avoid creating new files after every change in authority control of a file, ESeal files are appendable. Lastly, the client only needs to download the ESeals corresponding to their own identity and not the entirety of the file.\
