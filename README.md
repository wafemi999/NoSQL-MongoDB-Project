# NoSQL-MongoDB-Project
Illustration of aggregation pipelines in a document based DB

## Aim:

* To compute data with operations: $sort, $limit, $group, $sum, $min, $max, and $avg
* To build pipelines that generate useful insights about the data.




![collection_description](https://github.com/wafemi999/NoSQL-MongoDB-Project/assets/36579635/c440f07c-3327-425d-af26-862853a2aa70)

## Process

> start_mongo

* Connect to server:      
> mongo -u "username" -p "insert passwordd" --authenticationDatabase admin local

* only 2 documents from the marks collection
  >db.marks.aggregate([{"$limit":2}]) 

sorts the documents based on field marks in ascending order.
db.marks.aggregate([{"$sort":{"marks":1}}])

* descending
>db.marks.aggregate([{"$sort":{"marks":-1}}])
