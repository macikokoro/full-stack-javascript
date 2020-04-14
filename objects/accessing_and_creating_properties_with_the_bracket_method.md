# The Bracket Method

This method is similar to accessing array indices. We must pass in a string in order to reference a property.

`myFavoriteBook["author"];`

The bracket method comes in handy if we want to add a property name with spaces and characters.

`myFavoriteBook["Original Title"] = "Vingt mille lieues sous les mers";`

To use console.log with this type of method:

`console.log(myFavoriteBook["Original Title"]);`

Brackets also enable dynamic property access. Since they take expressions, we can avoid hard-coding every property access.

Lets create a function to add more chapters to our Object and to turn chapters into idividual Objects.

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
                       publicationDate: 1970,
                       "# of chapters": 0,
                       chapter1: {
                       };

function addBook ( book chapter title ){
    chapter
}
```

