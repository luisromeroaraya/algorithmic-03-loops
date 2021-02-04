# [Loops](https://github.com/becodeorg/BXL-Swartz-4-27/blob/master/1.The-Field/7.Algorithmic/03-loops.adoc)
* Type of challenge: **learning**
* Duration: **90 min**
* Team challenge: **solo**

## Learning objectives
At the end of this challenge you should:
* understand the concept of loops
* be able to write loops

## The mission
This challenge will have you play around with the concept of [loops](https://en.wikipedia.org/wiki/Control_flow#Loops), complete the exercises down below after you’ve read the explanations.

Ever had to repeat the same instructions multiple times in a row, look no further than the **loops**. They allow you to execute a piece of code multiple time or until a condition is met.

A *for loop* is usually used if you know how many iterations you need, a *while loop* iterates until a condition is met.

Example
```
// The output will be "0 ... 9" on a new line
for I = 0 until 9 do {
	output($I)
}

// Let's drink coffee
integer nbr_coffee = 10
boolean has_coffee = true
while ($has_coffee == true) do {
	drink_coffee()
	$nbr_coffee = $nbr_coffee - 1
	if ($nbr_coffee == 0) then {
		$has_coffee = false
	}
}
```

## Exercises

Instructions
* write your algorithm on paper
* detail each and every step
* indicates the types of used variables

*I will be using [Python3](https://repl.it/languages/python3) to write and test the algorithms*

I - print numbers
Write an algorithm which receives an integers *n* and prints:
- [x] the numbers from 1 to *n*
- [x] the numbers from 1 to *n* in descending order
- [x] the numbers from *-n* to *n*
- [x] the odd numbers from 1 to *n*
```
n=int(input("Please enter a number (1-10):"))

i=1
print("Numbers from 1 to", n, ":")
while i<=n:
    print(i)
    i=i+1

i=n
print("Numbers from", n, "to 1:")
while i>=1:
    print(i)
    i=i-1
i=n
print("Numbers from", n, "to", -1*n, ":")
while i>= (-1*n):
    print(i)
    i=i-1

i=1
print("Odd numbers from 1 to", n, ":")
while i<=n:
    print(i)
    i=i+2
```

II - print random number of integers
- [x] Write an algorithm which receives an random integer and prints from 0 to it.
```
import random
n=random.randint(1,10)

i=0
print("The numbers from 0 to",n,":")
while i <= n:
    print(i)
    i=i+1
```

III - throw dices
- [x] Write an algorithm which throws a dice a given number of times and count the number of times a certain number is received.
```
import random
t=int(input("Please enter given number of throws (1-100):"))
n=int(input("Please enter certain number to count (1-6):"))

total=0
i=1
while i <= t:
    dice=random.randint(1,6)
    i=i+1
    if dice == n:
        total=total+1

print("Total times number", n, "was thrown:", total)
```

IV - even numbers
- [x] Write an algorithm which prints all the even numbers from 0 to a given number.
```
n=int(input("Please enter a number (0-10):"))

i=0

print("Even numbers from 1 to", n, ":")
while i<=n:
    print(i)
    i=i+2
```

V - perfect number
- [x] Write an algorithm which verify if a given positive integer is a perfect number, meaning equal to the sum of his divisors (except himself).
```
n=int(input("Please enter a number to verify (1-100):"))
sum=0
i=1

while i<n:
    if n%i == 0:   
        sum=sum+i
    i=i+1

if sum == n:
    print("The number",n,"is perfect")
else:
    print("The number",n,"is not perfect")
```

Resources
* [conventions](https://github.com/becodeorg/BXL-Swartz-4-27/blob/master/1.The-Field/7.Algorithmic/conventions.adoc)
* [loops](https://computersciencewiki.org/index.php/Iteration)
