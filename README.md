# Problem Set 4
You should feel comfortable with GitHub by now. If you're not, come to office hours with me or the TAs.

The deliverables for this problem set are the following:

* `ps4-part1.py`
* `ps4-part2.py`

**Remember** I now expect you to write comments in your code! One point will be deducted if you do not provide comments explaining your code. Here's what I would like commented this time:

* Before every function, describe what it does and what its arguments are (if any).
* Before every variable, explain what value it is holding.

**Remember** Now at the top of very files, you will include your honor pledge. The first four lines (comments) of every Python file should be this information. You will lose one point if you don't include these four lines.

* The name of the file.
* Your name.
* The date.
* "This code is my own work. I did not share my code or look at the code of another student. I did not consult ChatGPT, CoPilot, or another large language model."

<~~! dictionaries, sets, tuples, modules (random), functions with return values you write yourself -->

## Part 1: Counting words in a file (dictionaries, tuples, functions with return values)
In this program you will read in a file, compile some statistics about the file, report those statistics to the user, and let the user ask about the frequencies of words and letters.

1. Write a function called `get_counts(filename)` that does the following:
   * Create an empty dictionary to store word counts called `word_counts`
   * Create an empty dictionary to store character counts called `char_counts`
   * Open the file and read the whole file into a string at once.
   * Split the string into a list of words using `split()`.
   * Go through that list of words, and use the `word_counts` dictionary to keep track of how many time you see each word.
   * Split the string into a list of characters using `list()`.
   * Go through that list of characters, and use the `char` dictionary to keep track of how many time you see each character.
   * Return the following as a tuple: `word_counts` and `char_counts`.
  
2. Write a `main()` function that does the following:
   * Ask the user to supply a file name. Remember that whatever file you want to read must be in the same directory as your program! I have supplied a file in this repo called `testfile.txt`. You can just use that.
   * Call `get_counts()` passing in the user's chosen file name as the argument. Remember when you call the function you need to save out what it returns as a variable. It will return the words counts and the char counts, so you'll need to call the function like this:

```
wc, cc = get_counts(thefilename)
```
  * Report back to the user the total number of words, the total number of characters, the total number of unique words, and the total number of unique characters. You can use the `keys()` and `values()` functions to get this information from your dictinoaries.
  * Then ask the user what word they want to know the count of, and report back that count (or 0 if the word is not in the dictionary).
  * Then ask the user what character they want to know the count of, and report back that count (or 0 if the character is not in the dictionary).

**USING INPUT** When you use `input()`, it doesn't automatically insert a space before what the user enters. You don't want the user entering a space themselves, so you have to put the space at the very end of whatever you put in quotes as the argument to `input()`.

Here is some sample output using the file `testfile.txt`.

```
Enter a file to process: testfile.txt
This file has 532 words.
This file has 3126 characters.
This file has 284 unique words.
This file has 60 unique characters.
What word count would you like to look up? the
The count of "the" is 37.
What character count would you like to look up? e
The count of "e" is 308.
```


## Part 2: Guess a random number (module)

## Part 3: Function that returns a tuple

