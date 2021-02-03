# Loops
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
```// The output will be "0 ... 9" on a new line
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

I will be using [Python3](https://repl.it/languages/python3) to write and test the algorithms

I - print numbers
Write an algorithm which receives an integers *n* and prints:
- [ ] the numbers from 1 to *n*
- [ ] the numbers from 1 to *n* in descending order
- [ ] the numbers from *-n* to *n*
- [ ] the odd numbers from 1 to *n*

II - print random number of integers
- [ ] Write an algorithm which receives an random integer and prints from 0 to it.

III - throw dices
- [ ] Write an algorithm which throws a dice a given number of time and count the number of time a certain number is received.

IV - even numbers
- [ ] Write an algorithm which prints all the even numbers from 0 to a given number.

V - perfect number
- [ ] Write an algorithm which verify if a given positive integer is a perfect number, meaning equal to the sum of his divisors (except himself).

Resources
* [conventions](https://github.com/becodeorg/BXL-Swartz-4-27/blob/master/1.The-Field/7.Algorithmic/conventions.adoc)
* [loops](https://computersciencewiki.org/index.php/Iteration)
