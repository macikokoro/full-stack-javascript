# Referencing Objects within Objects

To get to the deeper properties of an object within another object we can use dot extension or subsequent bracket notation.

```text
var myBookBox = { height: 8, length: 10, width: 12,
              book1: {title: "Strange Case of Dr Jekyll and Mr Hyde", author: "Robert Louis Stevenson"
}
```

Dot notation:

`console.log(myBookBox.book1.title);`

This logs out the Strange Case of Dr Jekyll and Mr Hyde.

Wit bracket notation: `console.log( myBookBox["book1"]["author"] );`

This logs out Robert Louis Stevenson.

