#Aim
To write a Python program to demonstrate list operations such as slicing, append, update, remove, extend, index, copy, concatenation, iteration, and clear.

#Algorithm

Step 1: Start the program.
Step 2: Create a list named Network containing elements like 5G, Up to 10Gbps, 6G, 1ms, VR/AR, 4G, Transport, etc.
Step 3: Print the complete list.
Step 4: Print a slice of the list from index 1 to 5.
Step 5: Add a new element to the list using append().
Step 6: Modify an element in the list using index assignment.
Step 7: Remove an element from the list using remove().
Step 8: Add multiple elements using extend().
Step 9: Find the index of an element using index().
Step 10: Create a copy of the list using copy().
Step 11: Concatenate the original list with the copied list.
Step 12: Traverse the list using a for loop.
Step 13: Traverse the list using a while loop.
Step 14: Remove all elements using clear().
Step 15: Print the list after clearing.
Step 16: Stop the program.

#Python Code

Network = ["5G","Up to 10Gbps","6G","1ms","VR/AR","4G","Transport",
           "Smart Factories","New Radio","mmwave","Sub-6 GHz",
           "Spectrum","Frequency bands"]
# Print list
print(Network)
# Slicing
print(Network[1:5])
# Append
Network.append("Twin")
print(Network)
# Update element
Network[4] = "WiFi"
print(Network)
# Remove element
Network.remove("Transport")
print(Network)
# Extend list
Network.extend(["Enable","Information"])
print(Network)
# Index
L = Network.index("5G")
print(L)
# Copy list
Network_copy = Network.copy()
print(Network_copy)
# Concatenation
con = Network + Network_copy
print(con)
# For loop
for i in Network:
    print(i)
# While loop
i = 0
while i < len(Network):
    print(Network[i])
    i += 1
# Clear list
Network.clear()
print("After clear:", Network)

#Output
['5G','Up to 10Gbps','6G','1ms','VR/AR','4G','Transport',...]
['Up to 10Gbps','6G','1ms','VR/AR']
['5G','Up to 10Gbps','6G','1ms','VR/AR','4G','Transport','Twin']
0
5G
Up to 10Gbps
6G
1ms
VR/AR
...
After clear: []
