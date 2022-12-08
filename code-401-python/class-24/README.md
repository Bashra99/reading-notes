# Hash Table

* **Hashing** is a technique that is used to uniquely identify a specific object from a group of similar objects

* Assume that you have an object and you want to assign a key to it to make searching easy. To store the key/value pair, you can use a simple array like a data structure where keys (integers) can be used directly as an index to store values. However, in cases where the keys are large and cannot be used directly as an index, you should use hashing.

## Hash function

* **Ahash function** is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.

* To achieve a good hashing mechanism, It is important to have a good hash function with the following basic requirements:

  * Easy to compute: It should be easy to compute and must not become an algorithm in itself.

  * Uniform distribution: It should provide a uniform distribution across the hash table and should not result in clustering.

* Less collisions: Collisions occur when pairs of elements are mapped to the same hash value. These should be avoided.

## Hash table

* A hash table is a data structure that is used to store keys/value pairs.
* It uses a hash function to compute an index into an array in which an element will be inserted or searched. By using a good hash function, hashing can work well.
* Under reasonable assumptions, the average time required to search for an element in a hash table is O(1).

## Collisions
A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.
 
## Applications

* Associative arrays: Hash tables are commonly used to implement many types of in-memory tables. They are used to implement associative arrays (arrays whose indices are arbitrary strings or other complicated objects).
* Database indexing: Hash tables may also be used as disk-based data structures and database indices (such as in dbm).
* Caches: Hash tables can be used to implement caches i.e. auxiliary data tables that are used to speed up the access to data, which is primarily stored in slower media.
* Object representation: Several dynamic languages, such as Perl, Python, JavaScript, and Ruby use hash tables to implement objects.
* Hash Functions are used in various algorithms to make their computing faster  