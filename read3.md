# Difference Between MySQL and NoSQL
MySQL is used in the SQL database management system, a product from Microsoft corporation, where in NoSQL is a database type where SQL is necessary to access the document-based contents of the non-relational database management systems. Structuring and standardizing the database is essential for a relational database with MySQL. NoSQL, on the other hand, allows the unformatted and non-related data to be placed and operated as per the user’s requirements.

## MySQL
* MySQL development project has made its source code available under the terms of GNU General Public License, also under a variety of proprietary agreements. Initially, MySQL was owned and sponsored by a Swedish company called MySQL AB, now owned by Oracle Corporation.
* MySQL is relational in nature since all the data is stored in different tables and relations are established using primary keys or other keys known as foreign keys.
* MySQL is fast, easy to use a relational database that is being utilized by big and small businesses equally well. There are a plethora of reasons behind the popularity of relational databases like MySQL. It is a very powerful program in its own right, by handling a large subset of the functionality of the most expensive and powerful database packages.
* A standard form of language being used is a well-known data language called SQL for MySQL database. It can work on a multitude of operating systems and with many languages like C++, PHP, Java, C, etc. One of the key advantages of MySQL is that it is customizable since open source GPL license allows programmers to modify the MySQL software to fit their own specific environments.
## NoSQL
  * A data structure used by the NoSQL database is vastly different from those used in a relational database. Some operations are faster in NoSQL than relational databases like MySQL. Data structures used by NoSQL databases can also be viewed as more flexible and scalable than relational databases.
  * A primary reason for this different data structure could be driven by the simplicity of design, simpler horizontal scaling to clusters of machines and more control over availability.
  * NoSQL databases are primarily used in big data and real-time web applications. These types of databases gain a surge in their popularity in the early twenty-first century. A primary reason for this sudden surge can say to be triggered by companies such as Facebook, Amazon, and Google.
  * Most of the NoSQL databases are driven by eventual consistency which means database changes are propagated to all nodes within milliseconds, so queries of data might not return updated data immediately, which is a problem called stale reads. A central concept of the NoSQL database revolves around “document”.
  * While every document-oriented database implementation differs on the details of the definition, but they all assume that documents encapsulate and encode data in some standard formats of encodings.
  * Documents are addressed in the database via a unique key that represents the document. In addition to the key lookup performed by a key-value store, the database also offered API or a query language that retrieves the documents based on their contents.
  [Docs](https://www.educba.com/mysql-vs-nosql/)
  ---
#  NoSQL Data Modeling Techniques	
There are two ways that you can start modeling your database. One is to Embed in the same document. Else, Seperate data in to another document and use as a reference in the other document. You must always try to store related data together in the same document.
**1st Approach : Embeding document**
```
{  
   "order_ID":"0001",
   "product":{  
      "product_name":"Pencil",
      "product_category":"office supplies",
      "list_price":"10.00"
   }
}
```
**2nd Approach : Refering document**
```
{  
   "order_ID":"0001",
   "product":"0002"
}{  
   "product_ID":"0002",
   "product_name":"Pencil",
   "product_category":"office supplies",
   "list_price":"10.00"
}
```

Now you would wonder what approach should you use in these type of senarios.

If you are trying to display or if you are required to show products details always along with the orders. the first approach is better.

If you have high no of reads attempts to the Order_Items document and the products are not required at all. then the second approach is better. Also notice that you no longer need to maintain product_ID fields with this approach. Those were used as database references (or foreign keys in relational database parlance) in the Order_Items document.

The key thing in designing is that the goal is to keep data that is frequently used together in the document.

Remember to use your queries as a guide to help strike the right balance of normalization and denormalization. Too much of either can adversely affect performance. Too much normalization leads to queries requiring joins. Too much denormalization leads to large documents that will likely lead to unnecessary data reads from persistent storage and other adverse effects.