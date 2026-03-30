
# SECTION - 1 :- LOOP BASICS (1-10)

# TASK - 1

from ast import pattern
from genericpath import exists


for i in range(1,50):
    print(i)

# TASK - 2
for i in range(1,100):
    if i % 2 == 0:
        print(i)

# TASK - 3

for i in range(1,100):
    if i % 2 != 0:
        print(i)

# TASK - 4

num=7
for i in range(1,11):
    print(num,"x",i,"=",num*i)

# TASK - 5

for i in range(1,101):
    print(i) 
sum_numbers=num * (num + 1) // 2
print("The sum of the first 100 numbers is:", sum_numbers)

# TASK - 6

for i in range(50,1,-1):
    print(i)
    
# TASK - 7    

for i in range(1,100):
    if i % 3 == 0 :
        print(i)

# TASK - 8

for i in range(1,10):
    if i % 4 == 0:
        print(i)  

# TASK - 9              

for i in range(1,10):
    if i % 6 == 0:
        print(i)

# TASK - 10     

n=int(input("enter a number: "))
print("The first", n, "numbers are:")
for i in range(1, n + 1):
    print(i)

# SECTION - 2 :-  WHILE LOOP (11-15)  

# TASK - 11  

num=20
while num <= 20:
    print(num)
    num += 1

# TASK - 12

factorial=1
while num > 0:
    factorial *= num
    num -= 1
print("The factorial of the number is:", factorial)

# TASK - 13

num=10
while num > 0:
    print(num)
    num -= 1

# TASK - 14 

num=15
count=0
while count <= num:
    print(count)
    count += 1

# TASK - 15

list=[]
while True:
    num = int(input("enter a number: "))
    if num == 0:
        break
    list.append(num)
print("The list of numbers entered is:", list)

# SECTION - 3 :- NESTED LOOPS (16-20)

# TASK - 16

rows=4
for i in range(1, rows + 1):
    for j in range(1, i + 1):
        print("*", end="")
    print()

# TASK - 17

rows=4
for i in range (1,5):
    for j in range(1, i+1):
        print(j, end="")
    print()

# TASK - 18

print("Multiplication Table:")
for i in range(1, 5):
    for j in range(1, 5):
        print(i * j, end="\t")
    print()

# TASK - 19

for i in range(3):
    print("A B C")

# TASK - 20

for i in range(1):
    print("1 2 3")
    for i in range(1):
        print("4 5 6")
        for i in range(1):
            print("7 8 9")  


# SECTION - 4 :- STRING BASICS (21-25)

# TASK - 21

def count_characters(string):
    count = 0
    for char in string:
        count += 1
    return count
string = "Hello, World"
print("The number of characters in the string is:", count_characters(string))

# TASK - 22

def count_vowels(string):
    vowels = "hello, world"
    count = 0
    for char in string:
        if char in vowels:
            count += 1
    return count
string = "Hello, World"
print("The number of vowels in the string is:", count_vowels(string))

# TASK - 23

def count_consonants(string):
    vowels = "hello, world"
    count = 0
    for char in string:
        if char.isalpha() and char not in vowels:
            count += 1
    return count

string = "Hello, World"
print("The number of consonants in the string is:", count_consonants(string))


# TASK - 24

def reverse_string(string):
    reversed_string = ""
    for char in string:
        reversed_string = char + reversed_string
    return reversed_string
string = "Hello, World"
print("The reversed string is:", reverse_string(string))

# TASK - 25

def is_palindrome(string):
    cleaned_string = string.replace(" ", "").lower()
    return cleaned_string == cleaned_string[::-1]
string = "A man a plan a canal Panama"
if is_palindrome(string):
    print("The string is a palindrome.")   
else:    print("The string is not a palindrome.") 


# SECTION - 5 :- STRING SLICING (26-30)

# TASK - 26

name="tirupathi"
print(name[0:5])

# TASK - 27

name="tirupathi"
print(name[6:9])

# TASK - 28

name="tirupathi"
print(name[ : :-1])

# TASK - 29

name="tirupathi"
print(name[ : :2])

# TASK - 30

name="tirupathi"
print(name[1:8:])


# SECTION - 6 :- LIST BASICS (31-35)

# TASK - 31

numbers = [1, 2, 3, 4, 5]
print(sum(numbers))

# TASK - 32

numbers = [1, 2, 3, 4, 5]
print(max(numbers))

# TASK - 33

numbers = [1, 2, 3, 4, 5]
print(min(numbers))

# TASK - 34

numbers = [1, 2, 3, 4, 5]
print(len(numbers))

# TASK - 35

numbers = [1, 2, 3, 4, 5]
element_to_find = 3
if element_to_find in numbers:
    print(f"{element_to_find} is present in the list.")
else:   
    print(f"{element_to_find} is not present in the list.")


# SECTION - 7 :- LIST OPERATIONS (36-40)


# TASK - 36

numbers=[1, 2, 3, 4, 5]
numbers.append(6)
numbers.append(7)
numbers.append(8)
print(numbers)

# TASK - 37

numbers=[1, 2, 3, 4, 5]
numbers.insert(2,9)
print(numbers)

# TASK - 38

numbers=[1, 2, 3, 4, 5]
numbers.remove(2)
print(numbers)

# TASK - 39

numbers=[1, 2, 3, 4, 5]
numbers_1=[]
for item in numbers :
    numbers_1.insert(0, item)
    print(numbers_1)


# TASK - 40

a = [76, 23, 45, 12, 54, 9]
n = len(a)

for i in range(n):
    for j in range(0, n - i - 1):
        if a[j] > a[j + 1]: 
            a[j], a[j + 1] = a[j + 1], a[j]

print(a)
