def fibonacci_sum_even(n):
    a, b = 0, 1
    total_sum = 0
    while a <= n:
        if a % 2 == 0:
            total_sum += a
        a, b = b, a + b
    return total_sum

# Taking user input for the maximum number in the Fibonacci sequence
max_num = int(input("Enter the maximum number in the Fibonacci sequence: "))

# Calculating the sum of even numbers in the Fibonacci sequence up to max_num
result = fibonacci_sum_even(max_num)
print(f"The sum of even Fibonacci numbers up to {max_num} is: {result}")
