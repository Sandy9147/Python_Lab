# Experiment 1: Verification of Algebraic and Bitwise Identities Using Python
Aim
To write a Python program to verify algebraic identities and bitwise identities using assignment operators.

Algorithm
Step 1: Start the program.
Step 2: Read two integer values a and b from the user.
Step 3: Verify the algebraic identity  
(a+b)² = a² + 2ab + b².
Step 4: Verify the algebraic identity  
(a-b)² = a² - 2ab + b².
Step 5: Verify the algebraic identity  
(a+b)(a-b) = a² - b².
Step 6: Verify the identity  
a³ + b³ = (a+b)(a²-ab+b²).
Step 7: Verify bitwise identity  
a|b = (a&b) + (a^b).
Step 8: Verify addition using bitwise operations.
Step 9: Verify subtraction using bitwise operations.
Step 10: Stop the program.

##Python Code

a = int(input("Enter a value: "))
b = int(input("Enter b value: "))

# 1 (a+b)^2 = a^2 + 2ab + b^2
LHS = (a+b)*(a+b)
RHS = (a*a) + (2*a*b) + (b*b)
print("The eq are", LHS == RHS)

# 2 (a-b)^2 = a^2 - 2ab + b^2
LHS = (a-b)*(a-b)
RHS = (a*a) - (2*a*b) + (b*b)
print("The eq are", LHS == RHS)

# 3 (a+b)(a-b) = a^2 - b^2
LHS = (a+b)*(a-b)
RHS = (a*a) - (b*b)
print("The eq are", LHS == RHS)

# 4 (a+b)(a+b) = 2(a^2-b^2)
LHS = (a+b)*(a+b)
RHS = 2*((a*a)-(b*b))
print("The eq are", LHS == RHS)

# 5 a^3 + b^3 = (a+b)(a^2-ab+b^2)
LHS = (a*a*a) + (b*b*b)
RHS = (a+b)*((a*a)-(a*b)+(b*b))
print("The eq are", LHS == RHS)

# Bitwise operations
# 1
LHS = a | b
RHS = (a & b) + (a ^ b)
print("The eq are", LHS == RHS)

# 2
LHS = a & (a | b)
RHS = (a | b) & a
print("The eq are", LHS == RHS)

# 3
LHS = b & (a | b)
RHS = (a | b) & b
print("The eq are", LHS == RHS)

# Addition identities
# 1
LHS = a + b
RHS = (a | b) + (a & b)
print("The eq are", LHS == RHS)

# 2
LHS = a + b
RHS = (a ^ b) + 2*(a & b)
print("The eq are", LHS == RHS)

# Subtraction identities
# 1
LHS = a - b
RHS = (a & (a ^ b)) - ((a | b) ^ a)
print("The eq are", LHS == RHS)

# 2
LHS = a - b
RHS = ((a | b) ^ b) - ((a | b) ^ a)
print("The eq are", LHS == RHS)

##Output
Enter a value: 20
Enter b value: 10
The eq are True
The eq are True
The eq are True
The eq are False
The eq are True
The eq are True
The eq are True
The eq are True
The eq are True
The eq are True
The eq are True
The eq are True
