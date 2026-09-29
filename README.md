# Python-Assignments
# 1. Print all prime numbers between input range (Ex - input 20 50, prints all prime numbers between 20 and 50).  

# Code
```
start = int(input("Enter starting number: "))
end = int(input("Enter ending number: "))

print("Prime numbers are:")

for num in range(start, end + 1):
    if num > 1:
        for i in range(2, num):
            if num % i == 0:
                break
        else:
            print(num, end=" ")
```
# Output
<img width="1043" height="292" alt="image" src="https://github.com/user-attachments/assets/739760f4-e615-4635-bacc-3a440a932006" />

# 2. Factorial using recursion  

# Code
```
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)

num = int(input("Enter a number: "))

if num < 0:
    print("Factorial is not defined for negative numbers")
else:
    print("Factorial:", factorial(num))
```
# Output
<img width="1038" height="285" alt="image" src="https://github.com/user-attachments/assets/273c75fa-4e96-4039-8767-dc8156216c92" />

# 3. Square of numbers using lambda  

# Code
```
square = lambda n: n * n
num = int(input("Enter a number: "))
print("Square:", square(num))
```
# Output
<img width="1022" height="163" alt="image" src="https://github.com/user-attachments/assets/34392a51-337a-44c7-a28b-671a3ac0d944" />

# 4. Find the second largest element in a list  

# Code
```
numbers = [10, 25, 8, 40, 30]
unique_numbers = list(set(numbers))
unique_numbers.sort()
if len(unique_numbers) >= 2:
    print("Second largest:", unique_numbers[-2])
else:
    print("Second largest element does not exist")
```
# Output
<img width="1018" height="158" alt="image" src="https://github.com/user-attachments/assets/cb860340-1a67-4ccf-8ad3-9458a4a8fc7d" />

# 5. Count frequency of characters in a string  

# Code
```
text = input("Enter a string: ")
frequency = {}
for char in text:
    if char in frequency:
        frequency[char] += 1
    else:
        frequency[char] = 1

print("Character frequency:", frequency)
```
# Output
<img width="1030" height="217" alt="image" src="https://github.com/user-attachments/assets/e408a63e-fcef-4285-91b3-f806324c690c" />

# 6. Calculate area of a circle using math library.

# Code
```
import math

radius = float(input("Enter the radius: "))

area = math.pi * radius * radius

print("Area of the circle:", round(area, 2))
```
# Output
<img width="1025" height="172" alt="image" src="https://github.com/user-attachments/assets/d9628123-1f3a-4e99-818f-fceedde48575" />

# 7. Reverse a string without using built-in reverse  

# Code
```
text = input("Enter a string: ")

reversed_text = ""

for char in text:
    reversed_text = char + reversed_text

print("Reversed string:", reversed_text)
```
# Output
<img width="330" height="125" alt="image" src="https://github.com/user-attachments/assets/37016e1a-d7ca-41d3-b229-37c711d0f347" />

# 8. Remove duplicates from a list  

# Code
```
numbers = [10, 20, 10, 30, 20, 40]
unique_numbers = []
for num in numbers:
    if num not in unique_numbers:
        unique_numbers.append(num)

print("Original list:", numbers)
print("List without duplicates:", unique_numbers)
```
# Output
<img width="545" height="201" alt="image" src="https://github.com/user-attachments/assets/e94eb693-0dc9-4499-b867-32797b62fa9b" />

# 9. Merge two dictionaries 

# Code
```
dict1 = {"name": "sriram", "age": 21}
dict2 = {"course": "CSE", "college": "Engineering College"}

merged_dict = {**dict1, **dict2}

print("Merged dictionary:", merged_dict)
```
# Output
<img width="722" height="216" alt="image" src="https://github.com/user-attachments/assets/3b7ed510-8392-490f-a706-452d1abacf20" />


# 10. Fibonacci series using recursion

# Code
```
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)

terms = int(input("Enter the number of terms: "))

if terms < 0:
    print("Please enter a non-negative number")
else:
    print("Fibonacci series:")

    for i in range(terms):
        print(fibonacci(i), end=" ")
```
# Output
<img width="1027" height="327" alt="image" src="https://github.com/user-attachments/assets/247f0e80-30b4-432d-b6d7-b7f3df63697f" />
