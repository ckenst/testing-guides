# Strings

> What are some interesting input tests for a simple string field?

## Strings

* Nothing
* Empty field \(clear the default value\)
* Null character \(ASCII 0\)
* Whitespace only \(tab, space, CR \(ASCII 13\), ASCII 127\)
  * `&nbsp;`
  * More available: https://en.wikipedia.org/wiki/Whitespace_character
* Hyphenated last names 
  * Rainbolt-greene
* Strings + Unicode
  * See emjois below
* Unicode like Emjois
  * Names like Chris 💣 (bomb)
  * [Awesome Unicode](https://github.com/Wisdom/Awesome-Unicode)  
* [Big List of Naughty Strings](https://github.com/minimaxir/big-list-of-naughty-strings)


## Uses

* eCommerce fields during checkout
* Forms