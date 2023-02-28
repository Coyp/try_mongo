# struct 

```c
table -> collection 
value -> documnent 

```


# insert 

```C
db.events.insert();

```


# get/find

```c

1. scan all
db.events.find({});
db.events.find({ $and($or): [ {}, {} ]});
db.numbers.find( {num: {"$gt"($lt $ne): 19995 }} )

2. show explain
db.numbers.find({num: {"$gt": 19995 }}).explain("executionStats")

```

# update 

```c
1. patch 
db.events.update({username: "smith"}, {$set: {country: "Canada"}})
  
2. overwrite
db.events.update({"usernme.firstname": "smith"}, {country: "Canada"})

3. patch array
$addToSet -> only add 
$push

4. find+patch
db.events.find().update_one();
db.events.find().update_many();
```

# delete 

```c
1. remove collection 
db.events.drop()

2. remove document 
db.events.remove({});
db.events.find().delete_one 
db.events.find({}).delete_many
```
