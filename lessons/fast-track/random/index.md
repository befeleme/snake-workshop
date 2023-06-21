> [warning]
> This is a machine-generated translation, meant to support the in-person workshop.

# Randomness

Sometimes it is necessary to select a random value. There is no function available directly in Python for this, but it can be accessed using the `import` command.

```pycon
>>> from random import randrange
>>> randrange(6)
3
```
Which means:
* From the `random` module (which contains functions related to random values), import the `randrange` function (which can select random numbers).
* Select a random number from six possibilities.

Call the `randrange` function multiple times. What numbers can you get?


{% filter solution %}
Numbers from 0 to 5 - not including 6.
Programmers count from zero, and when you count six numbers from zero,
you only get to five.

When you want to 'roll the dice' - select numbers from 1 to 6 - you can write:
```pycon
>>> from random import randrange
>>> randrange(6) + 1
4
```
{% endfilter %}

There are many modules like `random` from which useful extensions can be imported, for working with text, drawing images, working with files or days on the calendar, compressing data, sending emails, downloading from the internet... You just need to know (or be able to find) the name of the right module and function. And if what Python has built-in is not enough, additional extension modules can be installed.

## Random selection

When we're talking about chance, let's try to draw a random number in the lottery. From the list, we have the `random` module with the `choice` function to choose from.
```pycon
>>> from random import choice
>>> lotery = [3, 42, 12, 19, 30, 59]
>>> choice(lotery)
12
```

Similarly, you can choose a random card from your hand, a random participant in a course, a random color - anything you can put on a list.

## Summary

The command **import** provides you with functionality that is not directly available in Python.
The **random** module contains the **randrange** function (random number) and **choice** function (random element from a list).
