# Runes: baby steps with TDD

In this repo you can follow the step-by-step development of the `runes` example: a Go command-line utility to find Unicode characters by name.

Each step in the development is documented explaining the Go language features used in the code. We follow the TDD _(Test Driven Design)_ method, so we code a test and then implement the functionality being tested. This makes it easier to focus on the __what__ (the interface) before we think about the __how__ (the implementation).

You don't need to know Go to follow along. The only pre-requsite is to know programming in another language.


## Our goal

At the end of this tutorial, we'll have a command-line too which allows searching for Unicode characters, like emoji, by typing words that appear in the character name. For example:

```
$ runes face eyes
U+1F601	😁	GRINNING FACE WITH SMILING EYES
U+1F604	😄	SMILING FACE WITH OPEN MOUTH AND SMILING EYES
U+1F606	😆	SMILING FACE WITH OPEN MOUTH AND TIGHTLY-CLOSED EYES
U+1F60A	😊	SMILING FACE WITH SMILING EYES
U+1F60D	😍	SMILING FACE WITH HEART-SHAPED EYES
U+1F619	😙	KISSING FACE WITH SMILING EYES
U+1F61A	😚	KISSING FACE WITH CLOSED EYES
U+1F61D	😝	FACE WITH STUCK-OUT TONGUE AND TIGHTLY-CLOSED EYES
U+1F638	😸	GRINNING CAT FACE WITH SMILING EYES
U+1F63B	😻	SMILING CAT FACE WITH HEART-SHAPED EYES
U+1F63D	😽	KISSING CAT FACE WITH CLOSED EYES
U+1F644	🙄	FACE WITH ROLLING EYES
```

Give the `runes` command one or more words, and it returns a sorted list of all Unicode characters containing those words in their names.

To get started, go to the [project page](https://twgophers.github.io/runes/).


## Credits

This tutorial is based on the `charfinder` example from chapter 18 of [Fluent Python](http://shop.oreilly.com/product/0636920032519.do), by Luciano Ramalho. The Go version called `runefinder` was started in the [Garoa Gophers](https://garoa.net.br/wiki/Garoa_Gophers) study group: Afonso Coutinho (@afonso), Alexandre Souza (@alexandre), Andrews Medina (@andrewsmedina), João "JC" Martins (@jcmartins), Luciano Ramalho (@ramalho), Marcio Ribeiro (@mmr) and Michael Howard.
