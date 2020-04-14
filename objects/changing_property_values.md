# Changing Property Values

Dot notation or the dot operator also allows modification of properties, even when using methods.

Here is our book Object again.

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

To change the name of the author we could use:

`myFavoriteBook.author = "Bob";`

This would change the name of the author from Jules Verne to Bob.

With dot notation we can also modify the contents of a property.

`myFavoriteBook.contents.push("The Tantrums of Ned Land");`

Notice the use of the push method. This allows us to add or in this case push the missing chapters in our contents property.

