# reverse-a-number-without-using-strings-function-
def reverse_number(n):
    reversed_num = 0
    while n > 0:
        digit = n % 10  # Get the last digit
        reversed_num = reversed_num * 10 + digit  # Append digit to reversed_num
        n = n // 10  # Remove the last digit from n
    return reversed_num

# Get input from the user
number = int(input("Enter a number: "))

# Reverse the number
result = reverse_number(number)

# Display the result
print(f"The reversed number is {result}")
