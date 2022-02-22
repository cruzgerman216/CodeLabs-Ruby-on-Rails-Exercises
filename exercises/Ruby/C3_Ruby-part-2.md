# Ruby Exercises - Part 2

## READ BEFORE STARTING

**Use Git or GitHub Desktop to commit each exercise to GitHub** <br>

**Use a cloud based service or an IDE**<br>

**You can use one project for all exercises**<br>

**Exercise 2.0: Terminology** 
Copy and paste the contents of Part 2 in your README.md file.
``` 
.
.
.

## Part 2
<em>**Conditional**</em> - INSERT DEFINITION HERE <br>
<em>**The difference between if, elseif and else.**</em> - INSERT ANSWER HERE <br>
<em>**What are Case/When statements? </em> - INSERT DEfINNITION HERE <br>
<em>**What is a data structure? </em> - INSERT ANSWER HERE <rb>
<em>**Arrays**</em> - INSERT DEFINITION HERE <br>
<em>**What is meant by 'built-in' methods?**</em> - INSERT DEFINITION HERE <br>
<em>**Loops**</em> - INSERT DEFINITION HERE <br>
<em>**What are infinite loops?**</em> - INSERT DEFINITION HERE <br>
<em>**What is meant by 'built-in' methods?**</em> - INSERT ANSWER HERE <br>
## Part 3

## Part 4
```

- replace each <em>INSERT DEFINITION/ANSWER HERE</em> with the correct definition/answer in your own words. Using external resources are recommended.<br>

**Exercise 2.1: if/else Conditionals** <br>
Create a Ruby file called exercise-2.1.rb. 

1. Print out `What is your name?`. Get user input and store data in a variable called name.
2. Use an `if` statement to see if the name entered by the user is "john". If so, print out `I found you!`.
3. Use an `else` statement to print out `You're not who I'm looking for ` follow by the name the user entered.
4. Use the built in string method `downcase` to downcase all letters of the user input in case the user enters `JoHn`.
5. Change the print statement to `What is your first name?` Store user input in a variable. Add another print statement, `What is your last name?`. Store user input in a variable. Use the `if` statement to check to see if the first name is `john` and last name is `doe`. 
6. Add an `elsif` statement to check if the first name and last name equate to `amy jeans`. If so, print `Amy! Help me look for John Doe.`

**Exercise 2.2: Arrays and iterators** <br>
Create a Ruby file called exercise-2.2.rb. 

1. Create an array with numbers 1 through 10
2. Print out the first element of the array, the last element and its length.
3. Use `unshift` to add a number to the front of the array. Use `<<` to push a number to the end of the array.
4. Use a loop to print out each element of the array.
5. While iterating, multiply each number by 2.
6. If the result of the multiplication is an even number, print the result follow by ` is a even number`. 
7. If the result of the multiplication is an odd number, print the result follow by ` is a odd number`. 
8. Repeat lines 4-7 except, instead of a loop, use the built-in array method `select`.

**Exercise 2.3: More built in array methods** <br>
Create a Ruby file called exercise-2.3.rb. 

1. Print out the array built in methods

To see the methods
Example `puts [].methods`

1. Create an array with three strings that resemble names.
2. Use three different built in array methods that haven't been covered in this exercise. Googling is recommended.

**Exercises 2.4: Hashes** <br>
Create a Ruby file called exercise-2.4.rb. 

1. Set a variable called user to a hash with keys email and id. Store values for these keys.
2. Print the values with keys `email` and `id`. 
3. Choose and use three built in hash methods onto this object. 

To see the methods
`puts {}.methods`

Googling is recommended.

**Exercise 2.5: Printing user data**<br>
Create a Ruby file called exercise-2.5.rb.

Given the array of hashes:

```ruby 
users = [
    {
        name: "John Doe",
        age: 43
    },
    {
        name: "Amy Singer",
        age: 53
    },
    {
        name: "Jimmy Lendricks",
        age: 23
    }
]
```

Use a `while` loop to print the values of each hash such as "My name is ... and I am ...". If the first name starts with "Jimmy", print out "My name and age is confidential."

expected output: 
```
> My name is John Doe and I am 43.
> My name is Amy Singer and I am 54.
> My name and age is confidential.
```


**Exercises 2.6: Nested Loops** <br>
Create a Ruby file called exercise-2.6.rb.

Given the value: <br>
```
[[1,2,3],[[[4,5,6]]]]
```

Print each number in order. 

expected output: 

```
> 1
> 2
> 3
> 4
> 5
> 6

```

---

## Practice The Technical Interview
*Keep in mind, your skill level for solving algorithm challenges is separate from your skills in developing applications. In technical interviews, you may be told to solve these commonly used code challenges.*


**Exercise 2.7: FizzBuzz** <br> 
Create a Ruby file called exercise-2.7.rb. 

Write a program that prints the numbers from 1 to 100.
But for multiples of three print “Fizz” instead of the
number and for the multiples of five print “Buzz”. For
numbers which are multiples of both three and five
print “FizzBuzz”.

**Exercise 2.8: Valid Paranthesis ([leetcode](https://leetcode.com/problems/valid-parentheses/))** <br>
Create a Ruby file called exercise-2.8.rb. 

Given a string s containing just the characters '(', ')', '{', '}', '[' and ']', determine if the input string is valid.

An input string is valid if:

Open brackets must be closed by the same type of brackets.
Open brackets must be closed in the correct order.

Example 1: <br>

Input: s = "()" <br>
Output: true <br>

Example 2: <br>

Input: s = "()[]{}"  <br>
Output: true <br>

Example 3: <br>

Input: s = "(]" <br>
Output: false <br>

**Exercise 2.9: Roman to Integer ([leetcode](https://leetcode.com/problems/roman-to-integer/))** <br>
Create a Ruby file called exercise-2.9.rb. 

Roman numerals are represented by seven different symbols: I, V, X, L, C, D and M.

```
Symbol       Value
I             1
V             5
X             10
L             50
C             100
D             500
M             1000
```
For example, 2 is written as II in Roman numeral, just two one's added together. 12 is written as XII, which is simply X + II. The number 27 is written as XXVII, which is XX + V + II.

Roman numerals are usually written largest to smallest from left to right. However, the numeral for four is not IIII. Instead, the number four is written as IV. Because the one is before the five we subtract it making four. The same principle applies to the number nine, which is written as IX. There are six instances where subtraction is used:

I can be placed before V (5) and X (10) to make 4 and 9. 
X can be placed before L (50) and C (100) to make 40 and 90. 
C can be placed before D (500) and M (1000) to make 400 and 900.
Given a roman numeral, convert it to an integer.


Example 1:

```
Input: s = "III"
Output: 3
Explanation: III = 3.
```

Example 2:

```
Input: s = "LVIII"
Output: 58
Explanation: L = 50, V= 5, III = 3.
```
Example 3:

```
Input: s = "MCMXCIV"
Output: 1994
Explanation: M = 1000, CM = 900, XC = 90 and IV = 4.
```

---

:wave: Saw a mispelled word? Want to improve the class exercises? Create a **pull request** and **contribute**! 
