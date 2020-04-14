# Adding Properties

Even if an Object is already created, properties can continue to be added.

```text
var chapters = ["A Runaway Reef", "The Pros and Cons", "As Master Wishes",
                "Ned Land", "At Random!", "At Full Steam",
                "A Whale of Unknown Species", "Mobilis in Mobili",
                "The Tantrums of Ned Land"
                ];

var myFavoriteBook = { title: "Twenty Thousand Leagues Under the Sea",
                       author: "Jules Verne",
                       publisher: "Pierre-Jules Hetzel",
                       illustrator: "Alphonse de Neuville",
                       country: "France",
                       contents: chapters,
                       publicationDate: 1970
                       };
```

`myFavoriteBook.publicationDate = 1970;`

The book Object first attempts to look for a publicationDate property. If it doesn't find one, it creates one.

