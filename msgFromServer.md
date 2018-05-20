# Messages from Server
### init
发送给新加入的用户

``` js
{
    "a": "meta",
    "type": "init",
    "files": {
        "a.txt": {
            "activeUser": ['userId1', 'userId2'],
            "occupier": ['userId1', 'userId2'],
            "cursors": {
                'userId1': {
                    'row': 0,
                    'column': 30
                },
                'userId2': null
            }
        }
    }
    "users": {
        'userId1': {
            'id': 'userId1',
            'name': 'donggu',
            'color': '#66ccff'
        },
        'userId2': {
            'id': 'userId2',
            'name': 'kevinz',
            'color': '#0080FF'
        }
    },
    "data": [80,75,3,4,10,0,0,0,0,0,11,...,0,0,0],
    "portalId": "aaaa-bbbb-cccc"
}
```
~~另外还要发一下压缩包。~~**DONE**

### User Joined
当有新用户加入时广播其它用户

``` js
{
    'a': 'meta',
    'type': 'userJoined',
    'user': {
        'id': 'userId-2345678iujhbvcvgh',
        'name': 'Fanfan',
        'color': '#ffffff'
    }
}
```

### User Left
当用户退出时广播其它用户

``` js
{
    'a': 'meta',
    'type': 'userLeft',
    'userId': 'userId-uhhuiknj'
}
```

### Occupier Cleared

``` js
{
    "a": "meta",
    "type" : "occupierCleared",
    "path": "a.txt"
}
```

### File Closed

``` js
{
    "a": "meta",
    "type": "closeFile",
    "path": "a.txt",
    "userId": 'userId-dfswefv'
}
```

### Cursor Moved

``` js
{
    "a": "meta",
    "type": "moveCursor",
    "path": "a.txt",
    "cursor": {
        "row": 123,
        "column": 23
    },
    "userId": "userId-ijhy78iodiwjoje3"
}
```

### File Saved

``` js
{
    'a': 'meta',
    'type': 'saveFile',
    'path': 'a.txt',
    'userId': 'userid-vgbhnjmkm'
}
```

### New File

``` js
{
    'a': 'meta',
    'type': 'newFile',
    'path': 'a.txt',
    'userId': 'userid-vgbhnjmkm'
}
```

### Delete File

``` js
{
    'a': 'meta',
    'type': 'deleteFile',
    'path': 'a.txt',
    'userId': 'userid-vgbhnjmkm'
}
```

### Move File
重命名/移动文件

``` js
{
    'a': 'meta',
    'type': 'renameFile',
    'path': 'a.txt',
    'newPath': 'b.txt',
    'userId': 'userid-vgbhnjmkm'
}
