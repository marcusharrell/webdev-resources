# Strings! 🕸️
In JavaScript, Strings are values made up of text and can contain letters, numbers, symbols, punctuation, and even emojis!

**Strings in JavaScript are contained within a pair of either single quotation marks '' or double quotation marks ""**
<br><br>
Both quotes represent Strings but be sure to choose one and **STICK WITH IT.** If you start with a single quote, you need to end with a single quote. There are pros and cons to using both IE single quotes tend to make it easier to write HTML within Javascript as you don’t have to escape the line with a double quote.

```
'This is a string. 👏';

"This is the 2nd string. 💁";

```

## Enclosing Quotation Marks

Let’s say you’re trying to use quotation marks inside a string. You’ll need to use opposite quotation marks inside and outside of JavaScript single or double quotes. **That means strings containing single quotes need to use double quotes and strings containing double quotes need to use single quotes.**

```
"It's six o'clock.";

'Remember to say "please" and "thank you."';

```

Alternatively, you can use a backslash \ to escape the quotation marks. This lets JavaScript know in advance that you want to use a [special character](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String#escape_notation)

Here’s what that looks like reusing the examples above:
```
'It\'s six o\'clock.';

"Remember to say \"please\" and \"thank you.\"";

```

## String Methods and Properties
Strings have their own built-in variables and functions, also known as properties and methods. Here are some of the most common ones.

## String Length
A string’s length property keeps track of how many characters it has.
```
EXAMPLE
"caterpillar".length;

OUTPUT
11
```

### Source:
https://www.javascript.com/learn/strings
