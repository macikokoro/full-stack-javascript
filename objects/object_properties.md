# Referencing Properties

One way to peek at a property inside of an Object is to use dot notation.

Let's peek inside our book Object.

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

`myFavoriteBook.author; // -> "Jules Verne"`

This example returns the name of the author.

```text
myFavoriteBook.contents;
// -> ["A Runaway Reef", "The Pros and Cons", "As Master Wishes",
                "Ned Land", "At Random!", "At Full Steam",
                "A Whale of Unknown Species", "Mobilis in Mobili"]
```

The previous example returns the array inside chapters.

