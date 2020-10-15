# Hash Table

Hash Table is a data structure which stores data in an associative manner. In a hash table, data is stored in an array format, where each data value has its own unique index value. Access of data becomes very fast if we know the index of the desired data.

## Hashing

Hashing is a technique to convert a range of key values into a range of indexes of an array.

The most common hash table implementation uses chaining with linked lists to resolve collisions. This combines the best properties of arrays and linked lists.

Hash table operations are performed in two steps:

- A key is converted into an integer index by using a hash function.
- This index decides the linked list where the key-value pair record belongs.

![](https://yourbasic.org/algorithms/hash-table.png)

![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Hash_table_3_1_1_0_1_0_0_SP.svg/1200px-Hash_table_3_1_1_0_1_0_0_SP.svg.png)

![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Hash_table_5_0_1_1_1_1_1_LL.svg/450px-Hash_table_5_0_1_1_1_1_1_LL.svg.png)