# Json Demo

init:

```
{
  "a":"meta", 
  "type":"init",
  "userId":"tc",
  "portalId":"tp"
}
```



open file:

```
{
  "a":"meta", 
  "type":"openFile",
  "grammar":"javascript",
  "path":"tpa", 
  "userId":"tc"
}```



close file:

```
{
  "a":"meta", 
  "type":"closeFile",
  "path":"tpa",
  "userId":"tc",
  "newPath":"tpa2", //可空
  "newPosition": //如果newPath是null，则newPosition也为null
  {
    "row":1, 
    "column":2
  }
}```



move cursor:

```
{
  "a":"meta", 
  "type":"moveCursor",
  "path":"tpa",
  "userId":"tc",
  "newPosition":
  {
    "row":1, 
    "column":2
  }
}```



change to active:

```
{
  "a":"meta", 
  "type":"activate",
  "path":"tpa",
  "isActiveUser":true
}```



change grammar:

```
{
  "a":"meta",
  "type":"changeGrammar",
  "path":"tpa",
  "userId":"tc",
  "grammar":"java"
}```


