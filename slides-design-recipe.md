<!-- $theme: gaia -->

# A design recipe for functions
# :bulb:
### PyLadies Atlanta
### January 2017
##### Emily Reese :globe_with_meridians: eareese.com

---
## *Program by Design*

### programbydesign.org/overview

> One of the most pressing problems that the beginning student of programming (or of any other creative art) encounters is what we call the Blank Page Syndrome: the student, given a problem statement, confronts a blank page...and doesn't know how to begin.

---

# Blank Page Syndrome?
# :open_book:

---

# Why the design recipe?

* **Problem-solving requires synthesis.** Good programming takes more than memorizing syntax rules and what's available in the standard library.
* **Code is communication** -- with the computer, with other people, even with oneself in the future.
* Overcoming **BPS** :open_book:
  - Getting started
  - Getting unstuck

---

# Steps of the design recipe
# :clipboard:

---

# :clipboard: Step 1. Data definition
* How is the important information represented?
* What are the input(s) and output?

```python
""" Step 1. Design recipe example: f_to_c

Data definitions:

A Temperature is a Number.

Input: Temperature in F
Output: Temperature in C

"""
```
---

# :clipboard: Step 2. Specification

* **Contract**
  - Write contract based on data definitions
* **Purpose statement**
  - Write out the purpose of the function in full sentences
* **Examples**
  - Make up examples that demonstrate the expected output

Remember give the function a **name**.

---
# :clipboard: Step 2. Specification

```python
""" Step 2. Design recipe example: f_to_c

Contract:
Number -> Number

Purpose statement:
This function takes a temperature measured in Fahrenheit,
and returns the equivalent Celsius temperature.

Examples:
f_to_c(32) -> 0
f_to_c(212) -> 100
f_to_c(-40) -> -40

"""
```

---

# :clipboard: Step 3. Implementation
Time to define the function.

```python
""" Step 3. Design recipe example: f_to_c """

def f_to_c(temp):
  return temp
```
When writing the body of the function, it's better to write an *__incorrect__ implementation that __fulfills the contract__ from earlier steps* of the recipe, than to try and write a completely correct implementation.

---

# :clipboard: Step 4. Testing

Turn the examples from Step 2 into working tests.

```python
""" Step 4. Design recipe example: f_to_c
Examples:
f_to_c(32) -> 0
f_to_c(212) -> 100
f_to_c(-40) -> -40
"""
def f_to_c(temp):
  return temp
  
  
assert(f_to_c(32) == 0)
assert(f_to_c(212) == 100)
assert(f_to_c(-40) == -40)
```
---

# :clipboard: Step 5. Review

* Review test results
* Refactor the function body
* Repeat as needed

### Wishlist

Find yourself wishing you had a certain function as you review? Make a "function wishlist" and keep following the recipe to design each of them. :star2:

---

# Case study

### Design recipe example: `f_to_c`
* Complete example: https://repl.it/FVTM/2

### Design recipe practice: 
##### Project Euler problem 1
* Prompt: https://projecteuler.net/problem=1
* Template: https://repl.it/FVUr/3

---

# The end
# :comet: