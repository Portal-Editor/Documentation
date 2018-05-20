# Message from Client

init:

```javascript
{
  "a": "meta", 
  "type": "init",
  "userId": "tc",
  "name": "tn"
  "portalId": "tp"
}
```



open file:

```javascript
{
  "a": "meta", 
  "type": "openFile",
  "grammar": "javascript",
  "path": "tpa"
}
```



close file:

```javascript
{
  "a": "meta", 
  "type": "closeFile",
  "path": "tpa"
}
```



move cursor:

```javascript
{
  "a": "meta", 
  "type": "moveCursor",
  "path": "tpa",
  "newPosition":
  {
    "row":1, 
    "column":2
  }
}
```



change to active:

```javascript
{
  "a": "meta", 
  "type": "changeActiveStatus",
  "path": "tpa",
  "isActiveUser": true
}
```



change grammar:

```javascript
{
  "a": "meta",
  "type": "changeGrammar",
  "path": "tpa",
  "userId": "tc",
  "grammar": "java"
}
```

save file:

```javascript
{
  "a": "meta",
  "type": "saveFile",
  "path": "tpa"
}
```

create file:

```javascript
{
  "a": "meta",
  "type": "createFile",
  "path": "tpa",
  "isFolder": true
}
```


