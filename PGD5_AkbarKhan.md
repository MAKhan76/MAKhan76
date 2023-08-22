- 👋 Hi, I’m @MAKhan76
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

##Question 1: Basic List Operations
    ## a) Create a list named `fruits` containing the following items: "apple", "banana", "orange", "grape", "kiwi".
    
fruits = ["apple", "banana", "orange", "grape", "kiwi"]
print(fruits[2])
orange
## b) Add "pear" to the end of the list.

fruits.append('pear')
print(fruits)
['apple', 'banana', 'orange', 'grape', 'kiwi', 'pear']
## c) Insert "mango" at the second position in the list.

fruits.insert(1,"mango")
print(fruits)
['apple', 'mango', 'banana', 'orange', 'grape', 'kiwi', 'pear']
## d) Remove "orange" from the list.

fruits.remove("mango")
print(fruits)
['apple', 'banana', 'orange', 'grape', 'kiwi', 'pear']
## Question 2: Slicing and Indexing
## a) Create a list named `numbers` containing the integers from 0 to 9.

Numbers = [0,1,2,3,4,5,6,7,8,9]

print(Numbers)
print(type(Numbers[1]))
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
<class 'int'>
## b) Print the element at index 3.
print(Numbers[3])
3
## c) Print a sublist containing the elements from index 2 to 6 (inclusive).
print(Numbers[2:6])
[2, 3, 4, 5]
## d) Print the last three elements using negative indexing.

print(Numbers[-1:-4:-1])
[9, 8, 7]
## Question 3: List Comprehension
## a) Create a list named `squares` using a list comprehension that contains the squares of numbers from 1 to 10.

squares = list(range(1,11))

print(squares)
               
               
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
## b) Create a new list named `even_squares` using a list comprehension that contains the squares of even numbers from the `squares` list.


even_squares = squares[1:10:2]

print(even_squares)

# Use list comprehension to square each element

squared_list = [num ** 2 for num in even_squares]

print(squared_list)
[2, 4, 6, 8, 10]
[4, 16, 36, 64, 100]
## a) Create a list named `colors` containing the following items: "red", "green", "blue", "yellow", "purple".

colors = ["red", "green", "blue", "yellow", "purple"]

print(colors)
['red', 'green', 'blue', 'yellow', 'purple']
## b) Swap the first and last elements of the list.

indx0 = 0
indx4 = 4

colors[indx0],colors[indx4] = colors[indx4],colors[indx0]

print(colors)
['purple', 'green', 'blue', 'yellow', 'red']
## c) Reverse the order of the list.

colors = ["red", "green", "blue", "yellow", "purple"]

colors.reverse()
 
print(colors)


# Reverse the list using slicing
reversed_string_list = colors[::-1]

print(reversed_string_list)
['purple', 'yellow', 'blue', 'green', 'red']
['red', 'green', 'blue', 'yellow', 'purple']
## d) Remove the second and third elements from the list.

colors = ["red", "green", "blue", "yellow", "purple"]

del colors[1]
del colors[1]
##del colors[1,2]
print(colors)
['red', 'yellow', 'purple']
## Question 5: Advanced Slicing

## a) Create a list named `letters` containing the letters from 'a' to 'j'.

letters = ['a', 'b', 'c', 'd', 'e', 'f','j']

print(letters)
['a', 'b', 'c', 'd', 'e', 'f', 'j']
##  b) Using slicing, create a new list `first_half` containing the first half of the `letters` list.

print(len(letters))

first_half = letters[0:round(len(letters)/2)]

print(first_half)
7
['a', 'b', 'c', 'd']
# c) Using slicing, create a new list 'last_three' containing the last three elements of the 'letters' list.
letters = ['a', 'b', 'c', 'd', 'e', 'f','j']

print(letters[(round(len(letters)/2)*-1)+1::])
['e', 'f', 'j']
# Question 6: Nested Lists

"""
a) Create a nested list named 'matrix' with the following rows:
   - [1, 2, 3]
   - [4, 5, 6]
   - [7, 8, 9]
"""

matrix = [[1,2,3], [4,5,6], [7,8,9]]
for i in matrix:
    print(i)
[1, 2, 3]
[4, 5, 6]
[7, 8, 9]
# b) Print the element in the second row and third column.

print(matrix[1][2])
6
# c) Use nested indexing to change the value at the second row and first column to 0.

matrix[1][0] = 0
for i in matrix:
    print(i)
[1, 2, 3]
[0, 5, 6]
[7, 8, 9]
 
