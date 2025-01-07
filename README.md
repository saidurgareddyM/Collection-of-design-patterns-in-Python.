# Collection-of-design-patterns-in-Python.
def uppercase_decorator(func):
    def wrapper(text):
        result = func(text)
        return result.upper()
    return wrapper

@uppercase_decorator
def greet(name):
    return f"Hello, {name}"

# Usage
print(greet("John"))  # Output: HELLO, JOHN
