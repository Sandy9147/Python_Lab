#Aim
To write a Python program to demonstrate tuple operations such as accessing elements, length of tuple, nested tuple, concatenation, membership test, and built-in functions.

#Algorithm

Step 1: Start the program.
Step 2: Create three tuples:
t1 = (1,2,3)
t2 = (230,36,200)
t3 = ("Apples","Banana","Watermelon","Dragon fruit")
Step 3: Print the original tuples.
Step 4: Access elements from tuples using index values.
Step 5: Find the length of each tuple using len() function.
Step 6: Create a nested tuple by combining t1 and t3.
Step 7: Perform concatenation of two tuples.
Step 8: Check membership using in operator.
Step 9: Take a fruit name from the user and check if it exists in the tuple.
Step 10: Use built-in functions like max(), min(), and sum() on a numeric tuple.
Step 11: Display the results.
Step 12: Stop the program.

#Python Code

# WAP program to demonstrate tuples
t1 = (1,2,3)
t2 = (230,36,200)
t3 = ("Apples","Banana","Watermelon","Dragon fruit")
print("Original Tuple:", t1, t2, t3)
# Accessing elements
print("First element of t1:", t1[0])
print("Second element of t2:", t2[1])
print("Third element of t3:", t3[2])
# Length of tuple
print("Length of tuple1:", len(t1))
print("Length of tuple2:", len(t2))
print("Length of tuple3:", len(t3))
# Nested tuple
nested_tuple = (t1, t3)
print("Nested Tuple:", nested_tuple)
# Concatenation
t4 = t2 + t3
print("Concatenation of t2 and t3:", t4)
# Membership test
print("Is 2 in t1?", 2 in t1)
print("Is mango in t3?", "mango" in t3)
# Using if-else
word = input("Enter a fruit name to check: ")
if word in t3:
    print(word, "is present in tuple")
else:
    print(word, "is not present in tuple")
# Built-in functions
numbers = (98,28,23,70,4,10,48,84,79)
print("Max value:", max(numbers))
print("Min value:", min(numbers))
print("Sum of values:", sum(numbers))

#Output

Original Tuple: (1, 2, 3) (230, 36, 200) ('Apples', 'Banana', 'Watermelon', 'Dragon fruit')
First element of t1: 1
Second element of t2: 36
Third element of t3: Watermelon
Length of tuple1: 3
Length of tuple2: 3
Length of tuple3: 4
Nested Tuple: ((1, 2, 3), ('Apples', 'Banana', 'Watermelon', 'Dragon fruit'))
Concatenation of t2 and t3:
(230, 36, 200, 'Apples', 'Banana', 'Watermelon', 'Dragon fruit')
Is 2 in t1? True
Is mango in t3? False
Enter a fruit name to check: apple
apple is not present in tuple
Max value: 98
Min value: 4
Sum of values: 444
