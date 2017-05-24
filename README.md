# elastcisearch 2.x commands
Delete an index type

remove by query .mapping for the type persists so perform a reindex
```{
  "query": {
    "match": {
      "_type": "my_index"
    }
  }
}
```


