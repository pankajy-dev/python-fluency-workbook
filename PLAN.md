# Python Fluency Plan

**Goal:** Recall syntax without hesitation, write Python confidently.  
**Timeline:** 2 weeks, ~30–45 min/day  
**Rule:** Read the concept, then close notes and solve the assignments from memory.

---

## Week 1 — Core Syntax

### Day 1 — Types, Variables, F-strings

**Concepts to recall:** `int`, `float`, `str`, `bool`, type casting, f-strings

**Assignments:**
1. Create variables of each type and print them with their type using `type()`.
2. Take two numbers as strings `"12"` and `"5"`, cast them to int, and print their sum.
3. Given `name = "Alice"` and `score = 95.5`, print: `Alice scored 95.5 out of 100 (grade: A)` using an f-string.
4. Write a one-liner that checks if `"42"` is a digit and converts it to int if so.
5. Print the result of `7 / 2`, `7 // 2`, and `7 % 2` — know what each returns.

---

### Day 2 — Lists, Tuples, Dicts, Sets

**Concepts to recall:** creation, indexing, slicing, common methods, iteration

**Assignments:**
1. Create a list of 5 fruits. Print the last two using slicing. Remove one item by value.
2. Swap the first and last elements of a list without using a temp variable.
3. Given `scores = [10, 20, 30, 40, 50]`, print the sum, max, and reversed list.
4. Create a dict of 3 people with their ages. Add a new person, update an age, delete one entry.
5. Given two lists `a = [1, 2, 3, 4]` and `b = [3, 4, 5, 6]`, find their intersection and union using sets.
6. Iterate over a dict and print each key-value pair as `name: age`.

---

### Day 3 — Control Flow

**Concepts to recall:** `if/elif/else`, `for`, `while`, `break`, `continue`, `pass`

**Assignments:**
1. Write a program that takes a number and prints "positive", "negative", or "zero".
2. Print all even numbers from 1 to 20 using a `for` loop and `continue`.
3. Use a `while` loop to find the first power of 2 greater than 1000.
4. Loop through `[1, 2, 3, "a", 5]` and stop (break) when you hit a non-integer.
5. FizzBuzz: for 1–30, print Fizz (div by 3), Buzz (div by 5), FizzBuzz (both), else the number.

---

### Day 4 — Functions

**Concepts to recall:** `def`, return, default args, `*args`, `**kwargs`, `lambda`

**Assignments:**
1. Write `greet(name, greeting="Hello")` that prints `Hello, Alice!`.
2. Write `total(*numbers)` that returns the sum of any number of arguments.
3. Write `display(**info)` that prints each key-value pair from keyword arguments.
4. Use a `lambda` to sort `["banana", "apple", "cherry"]` by string length.
5. Write a function that returns multiple values (e.g. min and max of a list) and unpack them.
6. Write a recursive function to compute factorial of n.

---

### Day 5 — Comprehensions

**Concepts to recall:** list/dict/set comprehensions, conditional comprehensions

**Assignments:**
1. Create a list of squares of numbers 1–10 using a comprehension.
2. From `[1, 2, 3, 4, 5, 6, 7, 8]`, extract only odd numbers using a comprehension.
3. Given a list of words, create a dict of `{word: len(word)}`.
4. Flatten `[[1, 2], [3, 4], [5, 6]]` into a single list using a nested comprehension.
5. From `[1, -2, 3, -4, 5]`, create a list that replaces negatives with 0.
6. Create a set of unique first letters from `["apple", "avocado", "banana", "blueberry"]`.

---

### Day 6 — Error Handling

**Concepts to recall:** `try/except/else/finally`, raising exceptions, multiple except blocks

**Assignments:**
1. Write a function `safe_divide(a, b)` that handles `ZeroDivisionError` and returns `None`.
2. Write code that tries to convert user input to int and handles `ValueError` gracefully.
3. Create a custom exception `NegativeValueError` and raise it when a function receives a negative number.
4. Write a `try/except/else/finally` block — print different messages in each block.
5. Read a file that doesn't exist and handle `FileNotFoundError` by printing a helpful message.

---

### Day 7 — Practice Day

Write these from scratch without referencing notes:

1. **Word frequency counter:** Given a sentence, return a dict of `{word: count}` sorted by count descending.
2. **Student grades:** Given a list of `(name, score)` tuples, print names of students who passed (score >= 60) in alphabetical order.
3. **Shopping cart:** Use a class with methods `add_item`, `remove_item`, `total`. Items have a name and price.
4. **Safe calculator:** A function that takes two numbers and an operator (`+`, `-`, `*`, `/`) and handles invalid input.
5. **Number pyramid:** Print a pyramid of numbers up to n rows.

---

## Week 2 — Useful Patterns

### Day 8 — Strings Deep-dive

**Concepts to recall:** `.split()`, `.join()`, `.strip()`, `.replace()`, slicing, `.upper/.lower`, `in`

**Assignments:**
1. Reverse a string using slicing.
2. Check if a string is a palindrome (ignore case and spaces).
3. Given `"  hello world  "`, strip whitespace and title-case it.
4. Split `"a,b,,c,d"` on commas, filter out empty strings, and rejoin with `" | "`.
5. Count how many times `"the"` appears in a sentence (case-insensitive).
6. Given a list of words, join them into a sentence with proper capitalization.

---

### Day 9 — File I/O

**Concepts to recall:** `open()`, modes (`r/w/a`), `with`, reading lines, writing

**Assignments:**
1. Write a list of 5 names to a file, one per line.
2. Read the file back and print each name with its line number.
3. Append two more names to the same file without overwriting it.
4. Read a file and count the total number of words across all lines.
5. Copy the contents of one file to another, converting all text to uppercase.

---

### Day 10 — Classes

**Concepts to recall:** `__init__`, `self`, instance methods, `@classmethod`, `@staticmethod`, inheritance, `super()`

**Assignments:**
1. Create a `Rectangle` class with `width` and `height`. Add `area()` and `perimeter()` methods.
2. Add a `__str__` method so `print(rect)` shows something useful.
3. Create a `Square` class that inherits from `Rectangle` (only needs one side).
4. Add a `@classmethod` called `from_string` that parses `"4x5"` and returns a Rectangle.
5. Create an `Animal` base class and two subclasses (`Dog`, `Cat`) that override a `speak()` method.

---

### Day 11 — Iterators & Generators

**Concepts to recall:** `iter/next`, `enumerate`, `zip`, `yield`, generator expressions

**Assignments:**
1. Use `enumerate` to print a list with 1-based index numbers.
2. Use `zip` to pair two lists into a dict.
3. Write a generator `countdown(n)` that yields from n down to 0.
4. Write a generator that yields only prime numbers up to n.
5. Use a generator expression to compute the sum of squares of even numbers 1–100.

---

### Day 12 — Decorators

**Concepts to recall:** functions as arguments, `*args/**kwargs` pass-through, `@` syntax, `functools.wraps`

**Assignments:**
1. Write a `@timer` decorator that prints how long a function took to run.
2. Write a `@log_calls` decorator that prints the function name and arguments each time it's called.
3. Write a `@retry(n)` decorator that retries a function up to n times if it raises an exception.
4. Apply two decorators to one function and observe the order they run.

---

### Day 13 — Useful stdlib Modules

**Concepts to recall:** `collections`, `itertools`, `os`, `pathlib`, `datetime`

**Assignments:**
1. Use `Counter` from `collections` to find the 3 most common words in a sentence.
2. Use `defaultdict` to group a list of `(name, city)` tuples by city.
3. Use `itertools.chain` to iterate over multiple lists as one.
4. Use `pathlib.Path` to list all `.txt` files in the current directory.
5. Use `datetime` to print how many days until New Year's Day 2027.

---

### Day 14 — Final Practice

Mixed problems — no hints, no notes:

1. **Anagram checker:** Given two strings, return `True` if they are anagrams.
2. **Most frequent item:** Write a function that returns the most common element in a list.
3. **File word stats:** Read a text file and print the top 5 most frequent words (ignore punctuation).
4. **Matrix transpose:** Given a 2D list, return its transpose using comprehensions.
5. **Fibonacci generator:** Write a generator that yields Fibonacci numbers indefinitely; print first 15.
6. **Class + decorator:** Create a `BankAccount` class, decorate the `withdraw` method to log every withdrawal.
7. **Chain of filters:** From a list of dicts (people with name/age/city), filter adults from a specific city, sort by name, print names.

---

## Cheat Sheet File

Keep `cheatsheet.py` in the root. After each day, add a 2–3 line snippet for syntax you blanked on. Review it before each session.
