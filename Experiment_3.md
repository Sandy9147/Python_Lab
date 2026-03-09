#Aim
To write a Python program to perform various string operations such as reverse, count, palindrome check, upper case, lower case, capitalize, swap case, and substring search.

#Algorithm
Step 1: Start the program.
Step 2: Input a string from the user.
Step 3: Reverse the string using slicing and display the result.
Step 4: Find the length of the string using len() and display it.
Step 5: Check whether the string is a palindrome by comparing it with its reverse.
Step 6: Convert the string into uppercase using upper() and display it.
Step 7: Convert the string into lowercase using lower() and display it.
Step 8: Capitalize the first letter of the string using capitalize().
Step 9: Change uppercase letters to lowercase and vice versa using swapcase().
Step 10: Input a substring and check whether it exists in the string.
Step 11: Display the result.
Step 12: Stop the program.

#Python Code

str = input("Enter a word: ")
# Reverse
print(str[::-1])
# Count
count = len(str)
print(count)
# Palindrome
if str == str[::-1]:
    print("Palindrome")
else:
    print("Not Palindrome")
# Upper case
print(str.upper())
# Lower case
print(str.lower())
# Capitalize
print(str.capitalize())
# Swap case
print(str.swapcase())
# Substring
sub = input("Enter substring: ")
if sub in str:
    print("Exists")
else:
    print("Doesn't exist")

#Output

Example:
Enter a word: Sandy
ydnaS
5
Not Palindrome
SANDY
sandy
Sandy
sANDY
Enter substring: nd
Exists
