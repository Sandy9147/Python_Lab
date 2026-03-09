#Aim
To write a Python program to demonstrate dictionary operations using a phonebook application.

#Algorithm

Step 1: Start the program.
Step 2: Create an empty dictionary called phonebook.
Step 3: Ask the user how many entries they want to add.
Step 4: Use a for loop to input name and phone number.
Step 5: Store the name and phone number in the dictionary.
Step 6: Display the complete phonebook.
Step 7: Ask the user to enter a name to search and use get() to find the phone number.
Step 8: Display dictionary values(), keys(), and items().
Step 9: Create a copy of the dictionary using copy().
Step 10: Add a new entry using update().
Step 11: Ask the user for a name to remove and delete it using pop().
Step 12: Remove the last inserted item using popitem().
Step 13: Display the final phonebook.
Step 14: Stop the program.

#Python Code

phonebook = dict()
number = int(input("How many entries do you need? "))
for i in range(number):
    name = input("Enter a name: ")
    phoneno = input("Enter a phone number: ")
    phonebook[name] = phoneno
print("\nFull Phonebook:")
print(phonebook)
print("\nUsing get():")
search_name = input("Enter name to search: ")
print(phonebook.get(search_name, "Not Found"))
print("\nUsing values():")
print(phonebook.values())
print("\nUsing keys():")
print(phonebook.keys())
print("\nUsing items():")
print(phonebook.items())
print("\nUsing copy():")
copy_phonebook = phonebook.copy()
print(copy_phonebook)
print("\nUsing update():")
phonebook.update({"K":"1234567890"})
print(phonebook)
print("\nUsing pop():")
remove_name = input("Enter name to remove: ")
print(phonebook.pop(remove_name, "Not Found"))
print("\nUsing popitem():")
print(phonebook.popitem())
print("\nFinal Phonebook:")
print(phonebook)

#Output 

How many entries do you need? 2
Enter a name: Sandy
Enter a phone number: 9876543210
Enter a name: Ravi
Enter a phone number: 9123456780
Full Phonebook:
{'Sandy': '9876543210', 'Ravi': '9123456780'}
Using get():
Enter name to search: Sandy
9876543210
Using values():
dict_values(['9876543210', '9123456780'])
Using keys():
dict_keys(['Sandy', 'Ravi'])
Using items():
dict_items([('Sandy', '9876543210'), ('Ravi', '9123456780')])
Using copy():
{'Sandy': '9876543210', 'Ravi': '9123456780'}
Using update():
{'Sandy': '9876543210', 'Ravi': '9123456780', 'K': '1234567890'}
Using pop():
Enter name to remove: Ravi
9123456780
Using popitem():
('K', '1234567890')

Final Phonebook:
{'Sandy': '9876543210'}
