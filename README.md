# \<simple-db-document\>

implementation of Polymer.AppStorageBehavior for reading and writing to SimpleDB documents

```
  <simple-db-document
    id='doc'
    db-name='myDB'>
  </simple-db-document>
```

```
saveMyObject(key, obj) {
  this.$.doc.key = key;
  this.$.doc.data = obj;
  this.$.doc.save();
}
```

# \<simple-db-query\>

```
<simple-db-query
  id='query'
  data='{{_list}}'
  db-name='myDB'>
</simple-db-query>
```

```
loadMyObjects() {
  this.$.query.execute();
}
```
