# Exercise 17: Crafting Mind-Blowing Prompts
## Test 1 
Llama3 8B Instruct

### Input: 
1. which are the clean code practices used in software development
2. which are the clean code practices used in software development with examples in python

### Output:
Here are some clean code practices used in software development with examples in Python:

1. **Separation of Concerns (SoC)**: Divide the code into layers or modules, each responsible for a specific task or functionality.

Example:
```
# Instead of having a single long function
def calculate_total_cost(order):
    # calculate subtotal
    subtotal = 0
    for item in order['items']:
        subtotal += item['price'] * item['quantity']
    # calculate tax
    tax = subtotal * 0.08
    # calculate total cost
    total_cost = subtotal + tax
    return total_cost

# Break it down into smaller functions
def calculate_subtotal(order):
    subtotal = 0
    for item in order['items']:
        subtotal += item['price'] * item['quantity']
    return subtotal

def calculate_tax(subtotal):
    return subtotal * 0.08

def calculate_total_cost(subtotal, tax):
    return subtotal + tax
```
2. **Single Responsibility Principle (SRP)**: Each module or function should have only one reason to change.

Example:
```
# Instead of having a function that does multiple things
def send_email(user):
    # send email
    # update user status
    # send notification
    pass

# Break it down into smaller functions
def send_email(user):
    # send email
    pass

def update_user_status(user):
    # update user status
    pass

def send_notification(user):
    # send notification
    pass
```
3. **Don't Repeat Yourself (DRY)**: Avoid duplicating code by extracting common logic into reusable functions or modules.

Example:
```
# Instead of having multiple functions that do the same thing
def calculate_area_rectangle(length, width):
    return length * width

def calculate_area_circle(radius):
    return 3.14 * radius ** 2

# Extract the common logic into a reusable function
def calculate_area(shape):
    if isinstance(shape, dict):
        if 'length' in shape and 'width' in shape:
            return shape['length'] * shape['width']
        elif 'radius' in shape:
            return 3.14 * shape['radius'] ** 2
    raise ValueError('Invalid shape')

# Use the reusable function
print(calculate_area({'length': 4, 'width': 5}))  # 20
print(calculate_area({'radius': 3}))  # 28.26
```
4. **KISS (Keep it Simple, Stupid)**: Keep the code simple and avoid unnecessary complexity.

Example:
```
# Instead of having a complex function with many conditions
def calculate_total_cost(order):
    if order['type'] == 'simple':
        subtotal = 0
        for item in order['items']:
            subtotal += item['price'] * item['quantity']
        tax = subtotal * 0.08
        return subtotal + tax
    elif order['type'] == 'complex':
        # complex logic
        pass
    else:
        raise ValueError('Invalid order type')

# Simplify the function
def calculate_total_cost(order):
    if order['type'] == 'simple':
        return sum(item['price'] * item['quantity'] for item in order['items']) * 1.08
    else:
        raise ValueError('Invalid order type')
```
5. **YAGNI (You Ain't Gonna Need It)**: Don't add features or code that you don't need right now.

Example:
```
# Instead of adding unnecessary features
def calculate_total_cost(order):
    # calculate subtotal
    subtotal = 0
    for item in order['items']:
        subtotal += item['price'] * item['quantity']
    # calculate tax
    tax = subtotal * 0.08
    # calculate total cost
    total_cost = subtotal + tax
    # add unnecessary feature
    if order['type'] == 'VIP':
        total_cost *= 1.1
    return total_cost

# Remove the unnecessary feature
def calculate_total_cost(order):
    # calculate subtotal
    subtotal = 0
    for item in order['items']:
        subtotal += item['price'] * item['quantity']
    # calculate tax
    tax = subtotal * 0.08
    # calculate total cost
    total_cost = subtotal + tax
    return total_cost
```
6. **Code organization**: Organize the code into logical folders, files, and modules.

Example:
```
# Instead of having a long file with many functions
# organize the code into logical folders and files
# app/
#   __init__.py
#   models/
#     user.py
#     order.py
#   controllers/
#     user_controller.py
#     order_controller.py
#   views/
#     user_view.py
#     order_view.py
```
7. **Naming conventions**: Use consistent naming conventions for variables, functions, and classes.

Example:
```
# Instead of using inconsistent naming conventions
# use consistent naming conventions
# snake_case for variable and function names
# PascalCase for class names

def calculate_total_cost(order):
    pass

class Order:
    pass
```
8. **Code commenting**: Add comments to the code to explain what it does, why it's necessary, and how it works.

Example:
```
# Instead of having uncommented code
def calculate_total_cost(order):
    # calculate subtotal
    subtotal = 0
    for item in order['items']:
        subtotal += item['price'] * item['quantity']
    # calculate tax
    tax = subtotal * 0.08
    # calculate total cost
    total_cost = subtotal + tax
    return total_cost
    # This function calculates the total cost of an order
    # It takes into account the subtotal and tax
    # The tax is calculated as 8% of the subtotal
```
9. **Testing**: Write unit tests and integration tests to ensure that the code works as expected.

Example:
```
# Instead of not writing tests
# write unit tests and integration tests
import unittest

class TestCalculateTotalCost(unittest.TestCase):
    def test_calculate_total_cost(self):
        order = {'items': [{'price': 10, 'quantity': 2}, {'price': 20, 'quantity': 1}]}
        self.assertEqual(calculate_total_cost(order), 60)

    def test_calculate_tax(self):
        subtotal = 100
        self.assertEqual(calculate_tax(subtotal), 8)

if __name__ == '__main__':
    unittest.main()
```
10. **Code refactoring**: Refactor the code regularly to improve its quality, performance, and maintainability.

Example:
```
# Instead of having a complex function
# refactor the code to make it simpler and easier to understand
def calculate_total_cost(order):
    subtotal = sum(item['price'] * item['quantity'] for item in order['items'])
    tax = subtotal * 0.08
    return subtotal + tax
```
These are just a few examples of clean code practices used in software development with Python. By following these practices, you can write high-quality code that is maintainable, efficient, and easy to understand.