# Psych9040-HW9
Psych9040 Homework 9 
Taylor Breddy
2024-04-01
The Exercise: Variance of an array
Write a program that asks the user to enter 5 numbers, and then prints the variance of those numbers.

For example:

Enter 5 numbers:
number 1: 5
number 2: 3.14
number 3: 1.23
number 4: 100
number 5: 0.01

The variance of [5.00, 3.14, 1.23, 100.00, 0.01] is 1528.72
A Sample Solution
The Code:
#coding exercise: Variance of an Array
#write a program that asks the user to enter 5 numbers, and then prints the variance of those numbers
def calculate_variance(numbers):
    n = len(numbers)
    mean = sum(numbers) / n
    variance = sum((x - mean) ** 2 for x in numbers) / n
    return variance

numbers = []
for i in range(1, 6):
    num = float(input(f"number {i}: "))
    numbers.append(num)
    
variance = calculate_variance(numbers)
print(f"The variance of {numbers} is {variance:.2f}.")
The Output:
number 1: 5
number 2: 3.14
number 3: 1.23
number 4: 100
number 5: 0.01
The variance of [5.0, 3.14, 1.23, 100.0, 0.01] is 1528.72.
