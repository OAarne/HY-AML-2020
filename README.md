# HY-AML-2020

An Anki deck for the advanced course in machine learning, held in Spring 2020 at the University of Helsinki.

I (Onni) am adding cards as I go along, no guarantees that the deck is in any way complete. It would be very much appreciated if you'd like to add more cards to the deck and share them, see the contributing section.

## What Anki? Why?

Anki is a piece of spaced repetition software (SRS). SRS let's you create flashcards, and then has you _repeatedly_ review them at optimally _spaced_ intervals, with the intervals between reviews growing exponentially as the information gets ever more deeply ingrained in long-term memory. Anki is free and open source.

For an extended explanation of why Anki and SRS in general are awesome, see Michael Nielsen's [Augmenting Long-term Memory](http://augmentingcognition.com/ltm.html).

As Nielsen puts it,

> The single biggest change that Anki brings about is that it means memory is no longer a haphazard event, to be left to chance. Rather, it guarantees I will remember something, with minimal effort. That is, Anki makes memory a choice.

## Installing

1. [Install Anki](https://apps.ankiweb.net/).
2. [Install the CrowdAnki plugin for Anki](https://ankiweb.net/shared/info/1788670778) to enable importing decks from GitHub. You'll have to restart Anki after installing the plugin for the rest of the steps to work.
3. In Anki, click File -> Import from GitHub and type in `oaarne/HY-AML-2020` and click OK.
4. You should now have the deck. To get new cards as I add them to the deck, you'll have to intermittently repeat step 3, which shouldn't mess with your reviews. But consider making a backup of your local progress anyway.

Additionally, you may wish to make an account at ankiweb.net to sync your progress, and install the AnkiDroid or AnkiMobile app for Android or iOS respectively.

## Contributing

There's a bunch of instructions for how to contribute in the [CrowdAnki readme](https://github.com/Stvad/CrowdAnki), but the minimal workflow goes like this:

1. Message me (Onni) on here or on Slack so that I can make you collaborator on the repo. Alternatively, make fork and a PR instead of pushing directly to master.
2. Clone this repo, or pull the latest changes if you've cloned it before.
3. Re-import the deck in Anki to make sure that it's up to date there too.
4. Make your additions to the deck, if you haven't already.
5. Export the deck into the repo, such that the deck.json file and media directory get overwritten.
6. Git push

### Basics of making Anki cards

#### Card types

Anki supports a number of different types of cards, the most important ones are

- Basic, which just has a front and a back.
- Basic and reversed card, which asks you to remember it both front to back and back to front
- And most interestingly, Cloze, which allows you to add (multiple) non-overlapping fill-in-the blanks. E.g. `{{c1::Fill}} in the {{c2::blank}}` will separately ask you to remember the verb and the object of that sentence. On desktop, Ctrl+Shift+C makes a selection a Cloze deletion.

#### Math

You can add MathJax to cards like so `\( \mathbb E[f(x)] \)` for inline math, or `\[ \frac 1 2 \]` for display mode math.

#### Pictures

You can add images, e.g. plots, to cards by just dragging the image file into the editor.

