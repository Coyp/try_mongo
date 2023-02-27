# struct 

```c
table -> collection 
value -> documnent 

```


# insert 

```C
db.events.insert();

```


# find

```c
1. find all 
db.events.find({});
db.events.find({ $and($or): [ {}, {} ]});

2. scan $gt $lt $ne
db.numbers.find( {num: {"$gt": 19995 }} )

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


```

# delete 

```c
1. remove collection 
db.events.drop()

2. remove document 
db.events.remove({});
```
