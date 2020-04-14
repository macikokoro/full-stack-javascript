# Creating Objects

There are several ways to create Objects in JS. One way is the Object literal. This is also the most often used.

`var myFavoriteBook = {};`

A set of curly brackets means to make a new Object. In this case it's an empty object with no properties.

To add a property create a name for the property using a string and then assign a value to it using a :

```text
var myFavoriteBook = { title: "Twenty Thousand Leagues Under the Sea",
                       author: "Jules Verne",
                       publisher: "Pierre-Jules Hetzel",
                       illustrator: "Alphonse de Neuville",
                       country: "France"
                       };
```

Properties can have arrays of values and also accept variables.

```text
var chapters = ["A Runaway Reef", "The Pros and Cons", "As Master Wishes",
                "Ned Land", "At Random!", "At Full Steam",
                "A Whale of Unknown Species", "Mobilis in Mobili"];

var myFavoriteBook = { title: "Twenty Thousand Leagues Under the Sea",
                       author: "Jules Verne",
                       publisher: "Pierre-Jules Hetzel",
                       illustrator: "Alphonse de Neuville",
                       country: "France",
                       contents: chapters
                       };
```

* Notice how we have a reference to the chapters inside the book Object.

