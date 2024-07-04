# python-2
def is_palindrome(word):
    return word.lower() == word.lower()[::-1]

# Example usage:
word = "racecar"
print(f"'{word}' is a palindrome: {is_palindrome(word)}")


def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)

# Example usage:
num = 5
print(f"{num}! = {factorial(num)}")


def fibonacci(n):
    fib_sequence = [0, 1]
    while len(fib_sequence) < n:
        next_num = fib_sequence[-1] + fib_sequence[-2]
        fib_sequence.append(next_num)
    return fib_sequence

# Example usage:
n_terms = 10
print(f"Fibonacci sequence ({n_terms} terms): {fibonacci(n_terms)}")



def is_armstrong(num):
    num_str = str(num)
    num_digits = len(num_str)
    total = sum(int(digit) ** num_digits for digit in num_str)
    return num == total

# Example usage:
number = 153
print(f"{number} is an Armstrong number: {is_armstrong(number)}")






def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    return a / b

# Example usage:
num1, num2 = 10, 5
print(f"Sum: {add(num1, num2)}")
print(f"Difference: {subtract(num1, num2)}")

