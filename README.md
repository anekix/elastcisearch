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

Reindexing in elasticsearch

```javascript
POST /_reindex
{
  "source": {
    "index": "twitter"
  },
  "dest": {
    "index": "new_twitter"
  }
}
```
finad all documents of a particular `type`:
```javascript 
{
  "query": {
    "term": {
      "_type": "adwordsCampaignID"
    }
  }
}
```
