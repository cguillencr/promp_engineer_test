# Exercise 12: Importance of correct wording

## Test 1 
Llama3 8B Instruct

### Input: 
List 15 animal in python

### Output:
I'm happy to help! However, I need to clarify that Python is a programming language, not a living creature. Therefore, it's not possible to list animals in Python.

But if you meant to ask for a list of 15 animals that can be represented as strings or variables in a Python programming language, I can provide you with an example. Here's a list of 15 animals that can be used as variable names or strings in Python:

1. Lion
2. Elephant
3. Gorilla
4. Kangaroo
5. Penguin
6. Koala
7. Monkey
8. Snake
9. Tiger
10. Bear
11. Wolf
12. Dolphin
13. Whale
14. Butterfly
15. Octopus

Please note that this is just an example and not an actual list of animals that can be executed in a Python program.


## Test 2 

### Input: 
create a script that list the animals in python

### Output:
Here is a simple Python script that lists the animals I provided earlier:
```
# Define a list of animals
animals = [
    "Lion",
    "Elephant",
    "Gorilla",
    "Kangaroo",
    "Penguin",
    "Koala",
    "Monkey",
    "Snake",
    "Tiger",
    "Bear",
    "Wolf",
    "Dolphin",
    "Whale",
    "Butterfly",
    "Octopus"
]

# Print the list of animals
print("Animals:")
for animal in animals:
    print(animal)
```
You can save this script to a file with a `.py` extension (e.g. `animals.py`) and run it using Python (e.g. `python animals.py`) to see the list of animals printed to the console.

Alternatively, you can also use the `print()` function to print the list of animals in a single line:
```
print("Animals:", *animals)
```
This will print the list of animals separated by commas.