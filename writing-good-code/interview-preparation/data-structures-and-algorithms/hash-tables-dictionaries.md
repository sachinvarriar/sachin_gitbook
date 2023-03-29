# Hash Tables/Dictionaries

<figure><img src="../../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>image courtesy: <a href="https://programmathically.com/dictionaries-tuples-and-sets-in-python/">https://programmathically.com/dictionaries-tuples-and-sets-in-python/</a></p></figcaption></figure>

Hash tables are seen a lot in databases, cache, etc.

Hash tables have keys, which acts as a index to memory. The key is associated with an index using a hash function.&#x20;

eg. consider a dictionary with name basket. You would like to add a value 10000 to the key "grapes" i.e., basket.grapes = 10000. Then the hash function will find an index for this key, value pair , lets say allocation 711. the location 711 will now have the key "grapes" and the value 10000 stored in it.

**Hash Function :** A hash function is a function that generates a value of fixed length for any input it gets. eg. md5, sha1, sha256



#### Why are hash tables better than arrays?

Insert, lookup, delete and search are O(1) time complexity for hash tables.

#### What is hash table collision?

With the hash function, there is a possibility that more than one key-value pairs can end up in the same memory location. This slows down the ability to retrieve data from the hash table. Once a collision has happened the lookup of datya from such a hash table becomes O(n)

A linked list can solve the issue of collision
