# Decentralized Storage

Nela decentralized storage It is a specialized KAD network optimized for efficient scalability and for encrypted file sharing and distribution.

Nela decentralized storage has the following properties:

1. All stored files are encrypted
2. A Simplified distributed hash table (DHT).
3. The EDFS header and body are split into two different files.
4. File header is append-able.

In EDFS decentralized storage, the DHT stores the hash index of the full body of the encrypted file rather than its blocks. Therefore, storage nodes in the network also store the integrity information of the blocks that they hold.&#x20;

When a node is searched, it returns the integrity information of the blocks that it contains. As a consequence, when downloading a file from the decentralized storage, the DHT needs to be searched once, resulting in increased efficiency.&#x20;

**File Header Append-ability, Key-Value Storage, and Selective Download**

For commercial applications, the ESeal file may be very large (for example, it may reach 100MB if a million people were to rent independently).&#x20;

Nela decentralized storage supports the use of key-value to store each ESeal item in the EDFS header. Additionally, in order to avoid having to create new files after every change in authority control of a file, headers are append-able.&#x20;

Lastly, EDFS supports that the client only needs to download the ESeals corresponding to the identities it holds.
