## What is Data Modelling?

Data modeling (data modelling) is the process of creating a data model for the data to be stored in a database. This data model is a conceptual representation of Data objects, the associations between different data objects, and the rules. Data modeling helps in the visual representation of data and enforces business rules, regulatory compliances, and government policies on the data. Data Models ensure consistency in naming conventions, default values, semantics, security while ensuring quality of the data. 

### Data Model

TheData Model is defined as an abstract model that organizes data description, data semantics, and consistency constraints of data. The data model emphasizes on what data is needed and how it should be organized instead of what operations will be performed on data. Data Model is like an architect's building plan, which helps to build conceptual models and set a relationship between data items. 

## Create, Read, Update, Delete

When we are building APIs, we want our models to provide four basic types of functionality. The model must be able to Create, Read, Update, and Delete resources. Computer scientists often refer to these functions by the acronym CRUD. A model should have the ability to perform at most these four functions in order to be complete. If an action cannot be described by one of these four operations, then it should potentially be a model of its own. 

The CRUD paradigm is common in constructing web applications, because it provides a memorable framework for reminding developers of how to construct full, usable models. For example, let’s imagine a system to keep track of library books. In this hypothetical library database, we can imagine that there would be a books resource, which would store book objects. 

## CRUD and REST

In a REST environment, CRUD often corresponds to the HTTP methods POST, GET, PUT, and DELETE, respectively. These are the fundamental elements of a persistent storage system.

Throughout the rest of the article, we will recommend standards and response codes that are typically followed by developers when creating RESTful applications. Conventions may differ so feel free to experiment with different return values and codes as you become comfortable with the CRUD paradigm.

Imagine we are working with a system that is keeping track of meals and their corresponding prices for a restaurant. Let’s look at how we would implement CRUD operations.

* The **database** is an organized collection of structured data to make it easily accessible, manageable and update. In simple words, you can say, a database in a place where the data is stored. The best analogy is the library. The library contains a huge collection of books of different genres, here the library is database and books are the data.
* **data model** : an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities.
* **CRUD**:Create, Read, Update, Delete 
* **schema** A database schema is the skeleton structure that represents the logical view of the entire database. It defines how the data is organized and how the relations among them are associated. It formulates all the constraints that are to be applied on the data.
* **Non SQL (No SQL)** - Databases that are not organized like a SQL database in tabs and rows. It is a mechanism for storage and retrieval of non-relational databases.
* **Object Relation Mapping (ORM)**: a programming technique for converting data between incompatible type systems using object-oriented programming languages.
