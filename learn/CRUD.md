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
db.events.find({});
db.events.find({ $and($or): [ {}, {} ]});
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
