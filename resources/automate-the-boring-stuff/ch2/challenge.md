# The Challenge

This section was all about flow control - using if/else statements. This will be the focus of this challenge but you'll need to know a few things to be able to do it.

## Python Files

The book has you using an interactive session of Python but, instead, you'll want to create a script. Simply create a file called `whatever-you-want.py`, add your Python Logic to it, and then run it with `python whatever-you-want.py`.

For this challenge, create a file called `thermometer.py`. For now, add `print("I am a thermometer")` and then ensure it works with `python thermometer.py`

> When done, push this file up to your GitHub Repository. You can put a message like `created thermometer.py`

## Taking Input

In a way much like the `print` statement, you can ask for user input. Simply replace `print` with `input` and store it as a variable. Here's an example:

```python
# Ask the user for their name and store it in a variable
name = input("What is your name? ")

# Append the strings together and print the output
print("Hello " + name)
```

Running this will look as follows:

```bash
$ python say_hello.py
What is your name? Jon
Hello Jon
```

Now, update your file such that the output will be as such:

```bash
$ python thermometer.py
What is the temperature today? 86
Wow! It is 86 degrees!
```

> When you’ve tested that this works, push your code to GitHub with a message like `added temperature input`

### Something to Note

When you take input in this way, the variable you store is going to be of a string type. This means if you do something like

```python
age = input("How old are you? ")

five_years_from_now = age + 5

print("Five years from now, you will be " + five_years_from_now)
```

The print statement will not do math but, instead, append "5" to the input string. As an example:

```bash
$ python age_addition.py
How old are you? 34
Five years from now, you will be 345
```

This is _not_ what we want. Instead, we want to convert the input to an Integer so the math works as expected

```python
age = input("How old are you? ")

# Convert the age to an Integer
age = int(age)

five_years_from_now = age + 5

print("Five years from now, you will be " + five_years_from_now)
```

Now it will do the math as expected and the output will be what you expect.

> Once this is working, commit and push your update to GitHub again: `handle math using int()`

## Putting it all Together

Now you're ready to do the challenge! What you should be able to do with all of this information is update `thermometer.py` such that it asks for the temperature and it reacts accordingly. Should the temperature be higher than 85, for example, it will say `Wow! X Degrees? It is so hot!`

Create the script such that it can handle:

- Below Freezing
- Super Cold
- A bit Cold
- Nice and Cool
- Nice and Warm
- A bit Hot
- Super Hot
- Crazy Hot

> When you're done with this file and have tested it, push it up and let me know!

### Bonus Challenge

Update the program to work with **Celsius** instead of Fahrenheit! You’ll need to convert the value, and also adjust the ranges for your categories. Try it on your own first — then look up the conversion formula if needed.
