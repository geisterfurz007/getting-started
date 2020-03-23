# Table of contents:

1. [How I got started with coding](#how-i-got-started-with-coding)  
2. [How I suggest you get started with coding](#how-i-suggest-you-get-started-with-coding)  
   1. [Picking a language](#picking-a-language)  
   2. [Learning the basics](#learning-the-basics)  
      1. [Variables and constants](#variables-and-constants)  
      2. [Conditions](#conditions)  
      3. [Loops](#loops)  
         1. [For loop](#for-loop)  
         2. [While loop](#while-loop)  
      4. [Functions](#functions)  
3. [Editor](#editor)  
4. [Core competences](#core-competences)  
   1. [Searching](#searching)  
   2. [Learn to read and understand code of others](#learn-to-read-and-understand-code-of-others)  
   3. [Don't hesitate to ask...](#don-t-hesitate-to-ask)  
   4. [Know your tools](#know-your-tools)  
5. [Example projects](#example-projects)  
   1. [FizzBuzz](#fizzbuzz)  
   2. [Commandline Calculator](#commandline-calculator)  
   3. [Project Euler](#project-euler)

# How I got started with coding
I learnt the basics of programming in school. Initially we used the drag-and-drop editor
[Scratch](https://scratch.mit.edu/projects/editor/) that uses blocks you can stick together to create a program.
This helped give a basic understanding what structures would be available later when working in a proper programming language
for example loops, conditions and functions which will be explained later in this document.

This is how a small Scratch program looks like that lets the sprite on the right walk a (rough) circle.

![Example Scratch program](https://i.stack.imgur.com/6HukM.png)

After Scratch we started writing actual code in the programming language Pascal in the IDE Lazarus which... I cannot recommend. I haven't used Pascal ever since and I recommend using a language to learn programming that you will actually use later on. It was a good bridge for me to move from the rather abstract Scratch blocks to actual written code but it hasn't been a great experience.

After that I started working with Java which has been the first language I really learned properly. Over the last two to three years I picked up JavaScript for website and app development as well as Dart for app development.

# How I suggest you get started with coding

This probably mostly depends on how you learn best. What works best for me is to set myself a project goal. This can be something simple like a small commandline program that adds to numbers or something more ambitious like a calculator with graphical user interface, it's really up to you! I will have a few suggestions further down below (if I don't forget them) but you are basically free to choose what you want to create.

## Picking a language
This is probably the biggest barrier for a lot of people. There is an incredible amount of options to chose from, if you ask in chat, chances are you will get 4 different answers from 4 different people. Generally Python and JavaScript are probably good ones to start and widespread so you can get a lot of help with a little research online. You can try to write your project in a few languages as well to see what feels better for you (I strongly dislike the Python syntax for example; others prefer it over the JavaScript one).

## Learning the basics
There are a few things that you should be fluent in with every language and that you will need no matter what your project is (unless it's the casual Hello world program). In the following section I will provide code examples for common things you will need in Python and JavaScript (in that order).

### Variables and constants
Think of these as named values. They are called variable if you can change them and constants if the value is set in stone. You will use them everywhere to store, reuse and push around values.

This for example is a small snippet of Python code to show use of a variable.
```py
variable_name = 7
print(variable_name)
```

The same thing in JavaScript looks like this:
```js
let variableName = 7;
console.log(variableName);
```

You will already note the small differences for example in naming convention and the semicolons in the end in the JavaScript snippet that are missing in the Python one. These syntax differences will be present in the other snippets of this document. As said earlier: Feel free to pick what feels better for you!

### Conditions
Usually in the form of "If something is true, do this, otherwise do that", conditions (or if-statements) allow you to conditionally run code.

Python example

```py
if variable_name == 7:
    print("Value is equal to 7")
else:
    print("Value is not equal to 7")
```

and again the corresponding JavaScript version:

```js
if (variableName === 7) {
    console.log("Value is equal to 7");
} else {
    console.log("Value is not equal to 7");
}
```

### Loops

Often you want to execute a section of code multiple times. Instead of copy-pasting the code multiple times, you put it in a loop.

#### For loop
If you want to run the code for a set number of iterations, you usually use a for loop

```py
for i in range(5):
    print(i)
```

```js
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

#### While loop
If you want to run the code as long as a condition is met, you usually use a while loop:

```py
variable_name = 0
while variable_name < 7:
    print(variable_name)
    variable_name += 1
```

```js
let variableName = 0;
while (variableName < 7) {
    console.log(variableName);
    variableName += 1;
}
```

### Functions
It will happen that you want to run a block of code in multiple places in your code that need other things to happen between them so you cannot use a loop. In this case, use a function which you can think of as a named block of code that you can call.

In the following examples, the top section defines the function and the last line is an example call to the function.

```py
def function_name():
    print("This code is run in a function")

function_name()
```

```js
function functionName() {
    console.log("This code is run in a function");
}

functionName();
```

To make things more useful, you can pass parameters to functions. The classic example is an add function to sum two numbers:

```py
def sum_two_numbers(a, b):
    return a + b

print(sum_two_numbers(1, 2))
```

```js
function sumTwoNumbers(a, b) {
    return a + b;
}

console.log(sumTwoNumbers(1, 2));
```

Now at this point there is a lot more to discover but I hope the above sections helped to give you a little insight to what you can expect!

# Editor

Obviously you have to write your code in something! Usually you either use a pluggable editor (which you can think of as mostly plain text editor with the ability to add plugins that provide tooling for different languages) or an IDE (Integrated Development Environment) which comes with a whole lot of useful features built-in. Depending on how much customizability and support for different languages you want, you might want to choose an editor over an IDE which might be directed towards a certain language. My suggestions for different IDEs / editors for different languages:

Language | IDE / Editor
---------|-------------
Java     |IntelliJ IDEA Community Edition
JavaScript | Visual Studio Code (VSCode)
Python | PyCharm Community Edition

Now those are only my choices! I am sure you can ask in coding chat for suggestions by others using the language you chose for ideas on which editor to use!


# Core competences

Now there are a few things that I think are crucial to software development:

## 1. Searching
You will face issues when working on your project that you want to find solutions for.   
"How do I read user input from the commandline in python" might work for google. "input python" is much shorter and chances are you will get the same result. Generally try to use the 2-4 main keywords of what you are searching for + the language or framework you are working in. This might not make a big difference in the beginning, the more this will make a difference.

Don't give up if the first search didn't turn up what you wanted. Try different keywords, different combinations and open the first few links and read through them. Even if they are not what you want now, they might be relevant later or show you stuff that you think is going to be useful further on!

Learn to read the documentation for your language. Once you know how to read and understand the docs for your preferred language (whether that might be [Python](https://docs.python.org/3/library/stdtypes.html?highlight=range#range), [MDN for JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else), the [JavaDocs](https://docs.oracle.com/en/java/javase/11/docs/api/java.base/java/lang/Object.html#toString()) or others) you will be able to quickly understand the purpose of functions and classes (I will leave that one for you to figure out for now ;) ) much more quickly than through reading through tutorial articles or W3Schools pages.

Click StackOverflow links! Ok, this might be too generalized but in many cases (when you are searching well) the first Stack Overflow link is pretty much guaranteed to contain a decent explanation with code that fixes or solves your issue.

## 2. Learn to read and understand code of others

When following the last paragraph of the above section, it is important that you don't auto-pilot copy-paste the code from the answer and pop it into your project, let it run, see it works and continue. Take the time to read the explanation in the answer (hoping there is one) and read and **understand** the code. This (for me at least) is the fastest way to pick up new knowledge. If you don't understand the use of a certain function or line of the code, return to section one ;)

## 3. Don't hesitate to ask...

... after you did your research! Read [this](https://meta.stackoverflow.com/revisions/261593/1) to see how much research you should do before asking people (it may or may not be slightly exaggerated but I guess you get the point).

Noone is going to chop your head off if you ask a question, but please do some research before it (as tempting as it might be to ask directly!). After that, don't be afraid to ask a question. And when you do ask a question, don't ask permission to ask a question, and you don't have to ask someone specific the question you have. It's a lot easier for everyone to answer the question if you ask what you're wondering (or what you're trying to achieve) than if you ask about asking a question. Especially when people are lurking in the chat, they are more likely to answer a question about programming than a question about questions about programming ;)

## 4. Know your tools

Now this is somewhat for later but you can boost your efficiency by knowing what your IDE, package-management, build-tools can do. Especially knowing the shortcuts and hotkeys in your editor can speed your development up! When you do something in your editor with your mouse, have a look if you can spot a keyboard shortcut noted next to what you ended up clicking and try to memorize it when you feel like it's something you will end up doing often (things like formatting your code, auto-complete, auto-fix of issues, etc). It will save you some time in the long shot when you are not waiting for your editor to popup with something after you moved your mouse somewhere to hover over a marking of your editor. But as said: It's something you can adapt over time and don't have to focus from the beginning.

# Example projects

## FizzBuzz
 - Make the obligatory FizzBuzz program! This is a fairly simple program used in interviews to filter out candidates that have no experience with programming. The rules are rather simple:
   - Print all numbers from 1 to 100
   - If the number is divisible by 3, print Fizz instead
   - If the number is divisible by 5, print Buzz instead
   - If the number is both divisible by 3 *and* 5, print FizzBuzz instead

## Commandline Calculator
 - Make a small commandline tool that takes two numbers as argument and prints the sum!
 - Change that tool to also accept an operator (-, *, /) and calculate the corresponding value.
 - Change that tool again to accept a variable amount of values so you can sum, subtract, multiply and divide a bunch of numbers.
 - Change that tool to request the input values from the user. You can for example accept values until the user puts in one of the four operators and then calculate the value.
 - Update the code to make sure that the user cannot put in "Coding sucks" (or anything else that is not a number) without getting an error and without the program crashing.

## Project Euler
And because I am absolutely horrible at creativity and coming up with ideas for programs to run, I can highly recommend [Project Euler](https://projecteuler.net). Project Euler is a collection of problems that end up creating a single, clearly defined result with (usually) increasing difficulty. The first problem for example is: "Find the sum of all the multiples of 3 or 5 below 1000.". You can read the problems without an account, to check your solution you have to create one however.