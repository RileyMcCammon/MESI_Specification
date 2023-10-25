This specification models multiple processor cores, each with its own cache, and specifies how these caches behave when performing read and write operations. The viewpoint of this specification is of a cache directory, a centralized component in a multiprocessor system that maintains the state of all cache blocks in the system. The address of the cache have been abstracted away and this behaves as if any read/write occurs on the same address.

The invariants state that whenever a core is in modified or exclusive state then no other core is in this state. It also says that the data of cores in shared state all are equivalent.

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Diagrama_MESI.GIF/440px-Diagrama_MESI.GIF)
