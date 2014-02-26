# MongoDB

MondoDB is an open-source document database, one of the most used NoSQL databases.

It is document oriented database with dynamic squemas, meaning that each entry can have different attributes. The documents are stored in JSON format.

![Logo](./img/mongodb_logo.png)

We are using MongoDB because NoSQL databases in general allow to save full documents in one single entry, removing the need for joining different tables when a query is made, which saves processing time. Also, it allows replication across LAN and WAN, and Auto-Sharding (storing data across multiple machines) for horizontal scaling.

This also introduces some problems. Data will not be normialized, and some filters will be harder to execute. Also, some opperations might take longer, like counting a list of elements in an entity.

MongoDB stores objects in collections. The concept of collection is equivalent to a table in SQL databases. But these do not have a stablished squema. Instead, every object can have different attributes. For instance, a recipe could have an attribute defining allergies information, while others do not. Also, because entities are built as JSON objects, they can have lists inside of them without needing to use a different collection.

For complex queries, MongoDB provides Index on any attribute for high performance. 


## Example

#### Entity

One example of a blog post stored in MobgoDB could be as follows:

```
 {
    “_id”          : “4da2c0e2e999fb56bf000002”
    “title”        : “Una introducción a MongoDB”,
    “body”         : “Lorem ipsum dolor sit amet…”,
    “published_at” : “2011-05-09T18:17:07-07:00”,
    “author_info”  : {
                       “_id”  : “4dc8919331c0c00001000002”
                       “name” : “Carlos Paramio”
                     },
    “tags”         : [“MongoDB”, “NoSQL”, “Bases de datos”]
    “comments”     : [
                       {
                         “author_info” : { “name” : “Jorge Rubira”, “email” : “email1@example.com” },
                         “body”        : “Test”,
                         “created_at”  : “2011-05-10T10:14:01-07:00”
                       },
                       {
                         “author_info” : { “name” : “Txema Rodríguez”, “email” : “email2@example.com” },
                         “body”        : “Otro test”,
                         “created_at”  : “2011-05-10T10:14:09-07:00”
                       }
                     ]
    “liked_by”     : [“4d7cf768e999fb67c0000001”, “4da34c62ba875a19d4000001”]
  }
```

#### Querying

- For attribute:

```
db.posts.find({‘title’ : ‘Una introducción a MongoDB
```

- For nested attribute:

```
db.posts.find({‘author_info._id’ : ‘4da2c0e2e999fb56bf000002’})
```

- For list attribute:

```
db.posts.find({‘tags’ : ‘MongoDB’})
```

There are more advanced options for querying, like special conditions. These can be found with a quick search on Internet or the official docs.


## MongoDB in Django

We are using Django non-rel with *Django MongoDB Engine* for this project. Because of that, we will not be using default MongoDB commands to manage the database, instead we are using Django model API with a few modifications to define collections, store and query data. More information can be found on Django's document in this section.

## References
- [MongoDB official website and overview](http://www.mongodb.org/)
- [MongoDB docs](http://docs.mongodb.org/manual/)
- [Introduction to MongoDB (Spanish)](http://www.genbetadev.com/bases-de-datos/una-introduccion-a-mongodb)
- [Django MongoDB Engine docs](http://django-mongodb-engine.readthedocs.org/)