# Class 30 Reading Notes

## Hash Tables

> Hash tables have keys and values to store information. Hash function evaluates the key and tells us where to store the info in the array.

- **Hash** - the result of an algorithm taking in a string and converting it to a value to determine the index of an array

- **Buckets** - what is contained in each index of the array (each index is a bucket) Each one has a key and a value.

- **Collision** - when more than one key gets hashed to the same location as another on the hash table. This is resolved by changing the initial state of the buckets - initialize a linked list in each bucket and their key/values will be stored as a node in a linked list.

- **Storing Values** - Hash maps accept the key, calculate the hahs of the key, use modulus to convert the hash into an array index, store the key WITH the value by appending both to the end of a linked list

- **Reading Values** - accept a key, calculate the hash, use modulus to convert the hash to an array index, use the index to access the short linkedList representing a bucket, search the bucket looking for a node with a key/value pair that matches the key given

- **Methods**
  - *set()* - once the index is determined, check if something already exists in the index, add the key/value pair

  - *get()* - find the index, iterate through the bucket to see if the key exists and return the value

  - *has()* - accepts a key and returns a boolean if the key exists

  - *keys()* - returns an array of unique hash keys

  - *hash()* - accepts a key as a string and returns the index of the array where the key/value should be placed

key:emma
value: phone#

hash(key) -> index
hash(emma)-> 3

hash(person)-> 1
hash(somebody)-> 3

- create a linked list if have two keys with the same index so we can chain multiple keys to the same index
- in the future can do hash(keyValue) -> function will spit out the index of that key