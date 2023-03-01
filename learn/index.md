# insert 

```c
db.numbers.createIndex({num: 1})

1. unique index 
db.numbers.createIndex({num: 1}, {unique:true})

2. sparse index 
db.numbers.createIndex({num: 1}, {unique:true, sparse:true)
```

# get 

```c
1. get all indexes
db.numbers.getIndexes()
```
