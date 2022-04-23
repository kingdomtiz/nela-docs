# DSCAN

Nela has built a Decentralized Security Content Acceleration Network called DSCAN. The core component of the DSCAN is the proxy/cache node, whose main function is to optimize the accessibility of files across the network. Proxy/cache nodes implement the following key features:

1. The proxy/cache node is a part of every storage node in the network. Essentially, every node in the network (beside L1 bridge providers) is both a storage and proxy/cache node.
2. When files are first uploaded to the network, they are saved whole on the proxy/cache nodes and are uploaded and copied whole to two or more proxy/cache nodes. Over time, proxy/cache nodes disseminate the file’s blocks across the storage nodes of the network.
3. The cache/proxy node automatically caches files retrieved for users so that the more popular a file is the more copies of it are cached on the DSCAN layer. As a result, the network nodes provide a multilayered architecture of cache and original storage.&#x20;

**It is key to note that users interacting with the system interact only with the proxy/cache layer of the network and the storage layer is accessed only through the proxy/cache layer.**&#x20;

When a user downloads a file to the network:

1. If the cache node contains the file in the cache, it serves the file.
2. Otherwise, the proxy/cache node will download the blocks of the file from storage nodes, serve the blocks to the user, and cache the complete file. The proxy/cache node will maintain the copy of the full file in the cache.



DSCAN makes EDFS decentralized storage superior to most if not all decentralized storage solutions currently available. Additionally, DSCAN:

1. Provides a more efficient, stable, and secure service for network access (a) Compared to traditional CDNs, the acceleration effect is correlated to the number of nodes. In DSCAN, since every node is also a proxy/cache node, the greater the network size, the greater the impact. (b) With backed-up content in the cache, service performance is greatly improved. (c) With the “three miles” of DSCAN acceleration, the overall user experience is improved.
2. Since cached content is encrypted by EDFS on the cache node, the acceleration/dissemination of the file in the network is secure and reliable.
3. Different users are directed to various nearby nodes, which are resistant to DDOS attacks. Traditional decentralized systems use XOR routing addressing, and the results are inaccurate. In DSCAN, routing is based on the actual detection RTT results, which seek the fastest path to synchronize data or services.
4. DSCAN is modular and can be extended by DApp to support other network protocols, such as IPFS. This enables network content acceleration to support more ecosystems flexibly.
