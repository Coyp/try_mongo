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
db.events.update({username: "smith"}, {country: "Canada"})

```
