# Hashtables

* Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.
* Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose.
* In the case of a hashtable, it is used to determine the index of the array.
* Buckets - A bucket is what is contained in each index of the array of the hashtable.
* Each index is a bucket.
* An index could potentially contain multiple key/value pairs if a collision occurs.
* Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.
* hashtable use to store the key into this data structure and quickly retrieve the value.
* hash map uses a “hash function” to place each item at a precise index location, based off it’s key.
* the hash function takes a key and returns an integer.
* We use the integer to determine where the key/value pair should be placed in the array.
* The hash code is used again to read something from the hash map.
* The hash table starts each bucket empty and overwrites their value once a key generates a hashCode that corresponds with an index.

## Collisions

* A collision occurs when more than one key hashes to the same index in an array
* the worst possible hash is one that hashes every single key to the same exact index of an array.
* Collisions are solved by changing the initial state of the buckets.
* Instead of starting them all as null we can initialize a LinkedList in each one
* if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list.
* Each index in the array is called a “bucket” because it can store multiple key/value pairs.

* Hash maps do this to store values:
  * accept a key
  * alculate the hash of the key
  * use modulus to convert the hash into an array index
  * store the key with the value by appending both to the end of a linked list

* Hash maps do this to read value:
  * accept a key
  * calculate the hash of the key
  * use modulus to convert the hash into an array index
  * use the array index to access the short LinkedList representing a bucket
  * search through the bucket looking for a node with a key/value pair that matches the key you were given