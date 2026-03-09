#Aim
To write a Python program to demonstrate looping statements using for loop and while loop.

#Algorithm

#Part A – For Loop (Multiplication Table)
Step 1: Start the program.
Step 2: Input a number n from the user.
Step 3: Use a for loop from 1 to 10.
Step 4: Multiply n × i in each iteration.
Step 5: Display the result.
Step 6: Stop the program.
#Part B – While Loop (Factorial)
Step 1: Start the program.
Step 2: Input a number n from the user.
Step 3: Initialize fact = 1 and i = 1.
Step 4: Repeat the loop while i ≤ n.
Step 5: Multiply fact = fact × i.
Step 6: Increment i by 1.
Step 7: Display the factorial value.
Step 8: Stop the program.

#Python Code

# For Loop - Multiplication Table
n = int(input("Enter a number: "))
for i in range(1,11):
    print(n*i)

# While Loop - Factorial
n = int(input("Enter a number: "))
fact = 1
i = 1
while i <= n:
    fact = fact * i
    i = i + 1
    print(fact)
    
#Output

Enter a number: 2
2
4
6
8
10
12
14
16
18
20

Enter a number: 4
1
2
6
24
