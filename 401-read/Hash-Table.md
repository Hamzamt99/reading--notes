# Hash Table
## What is Hash Table:
### A hash table, also known as a hash map, is a data structure used in computer science to store and retrieve key-value pairs efficiently. 
### It is commonly used to implement associative arrays or dictionaries, where each key maps to a corresponding value

## Why Hash Table:

### Hash tables offer several benefits that make them a popular and efficient choice for storing and retrieving data in various programming scenarios:

- Fast Data Retrieval: Hash tables provide constant-time average case complexity for common operations such as insertion, deletion, and retrieval. This means that the time it takes to perform these operations remains relatively constant, regardless of the size of the data set.

- Key-Value Storage: Hash tables are designed for storing key-value pairs, making them ideal for implementing data structures like dictionaries, maps, and associative arrays. This is especially useful when you need to associate unique keys with specific values.

- Efficient Searching: Hash tables use hash functions to map keys to specific memory locations, allowing for quick and direct access to values associated with keys. This significantly reduces the need for sequential searching through the entire data structure.

- Flexibility with Keys: Hash tables allow you to use a wide variety of data types as keys, including strings, numbers, and objects. This flexibility enables you to create efficient lookups for different types of data.

## How to use Hash Table:

```javascript
// Creating a hash table (object) and adding key-value pairs
const hashTable = {
  "key1": "value1",
  "key2": "value2",
  // ...
};

// Accessing values using keys
const value1 = hashTable["key1"];  // Retrieves "value1"
const value2 = hashTable["key2"];  // Retrieves "value2"

// Adding a new key-value pair
hashTable["key3"] = "value3";

// Deleting a key-value pair
delete hashTable["key2"];


// Adding a new key-value pair
hashTable["key3"] = "value3";

// Deleting a key-value pair
delete hashTable["key2"];
