# learn-ruby-lang

_This was created during my time as a student at [Code Chrysalis](https://www.codechrysalis.io)._

## Intro

## Common commands

| Command                                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                   | Example                                                                                                                   |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `puts`                                  | **put s**omething on the screen                                                                                                                                                                                                                                                                                                                                                                                                               | `puts "Hello World"                                                                                                       |
| `"foo".reverse`                         | a **method** to reverse a string; can't be used on numbers                                                                                                                                                                                                                                                                                                                                                                                    | `oof`                                                                                                                     |
| `123.to_s.reverse`                      | to reverse a number                                                                                                                                                                                                                                                                                                                                                                                                                           | `"321"` (_the value is now a string, not a number_)                                                                       |
| `"Travis".length`                       | a **method** to get length of string                                                                                                                                                                                                                                                                                                                                                                                                          | `6`                                                                                                                       |
| `"word" * 2`                            | repeats a string                                                                                                                                                                                                                                                                                                                                                                                                                              | `wordword`                                                                                                                |
| `to_s`                                  | converts things to strings                                                                                                                                                                                                                                                                                                                                                                                                                    |
| `to_i`                                  | converts things to integers                                                                                                                                                                                                                                                                                                                                                                                                                   |
| `to_a`                                  | converts things to arrays                                                                                                                                                                                                                                                                                                                                                                                                                     |
| `[10, 5, 20].sort!`                     | sort an array; the **`!`** is called a **`bang method`** and indicates that the original value is being permanently changed. (Bangs 💇 and methods) should be used with caution                                                                                                                                                                                                                                                               | `[5, 10, 20]`                                                                                                             |
| `poem.gsub("oldWord", "newWord")`       | **g**lobal **sub**stitute. Replacees all instances of `oldWord` with `newWord` inside `poem`.                                                                                                                                                                                                                                                                                                                                                 |
| `puts poem.lines.reverse.join`          | Imagine a poem with 3 lines. `lines` takes each line and adds them to an array with `\n` at the end of each value. `.reverse` reverses the order of the items in the array. The `join` method took that array of lines and put them together into a string. This is called **method chaining**                                                                                                                                                | poem = Roses are red<br>Violets are Blue<br>I love you<br><br>Result =<br>I love you<br>Violets are Blue<br>Roses are red |
| `books = {}`                            | creates a `hash` called "books". A hash is like an array, only every one of its elements has a name                                                                                                                                                                                                                                                                                                                                           |
| `books["Little Women"] = :splendid`     | add something to a `hash`. Note that the book title goes inside `[""]` and the book rating is a `symbol` after the equal sign.                                                                                                                                                                                                                                                                                                                |
| `:splendid`                             | created a `symbol` called "splendid". Symbols are cheaper than strings (in terms of computer memory.) If you use a word over and over in your program, use a symbol. Rather than having thousands of copies of that word in memory, the computer will store the symbol only once. More importantly, a symbol tells you that this is not just any old word but has a meaning within your program.                                              |
| `puts books["Little Women"]`            | retireve from a `hash` using the item's title.                                                                                                                                                                                                                                                                                                                                                                                                | returns `splendid`                                                                                                        |
| `books.keys`                            | returns all `keys` in the "books" `hash`.                                                                                                                                                                                                                                                                                                                                                                                                     | `["Little Women", "Harry Potter"]`                                                                                        |
| `books.values`                          | see the values from the `hashs`                                                                                                                                                                                                                                                                                                                                                                                                               | `["splendid", "magical"]`                                                                                                 |
| `3.times { print "mkay... " }`          | `{}` indicate a `block`. Blocks are always attached to methods. Like the times method, which takes the block and runs the code over and over. (In this example: three times.)                                                                                                                                                                                                                                                                 | `mkay... mkay... mkay...`                                                                                                 |
| `5.times { \|time\|` <br> `puts time }` | As we saw in the first example with a block (when counting ratings) we can pass a value to the block. Which values are passed is determined by the method that is running the block. The values that are received by the block are placed in the variable name at the beginning of the block, between two pipe symbols. Here, method `.times` sends a value to variable \|time\|. But note that variable time is only known within the block. | `0` <br> `1` <br> `2` <br> `3` <br> `4`                                                                                   |
