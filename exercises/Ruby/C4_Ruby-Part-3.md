# Ruby Exercises - Part 3

## READ BEFORE STARTING

**Use Git or GitHub Desktop to commit each exercise to GitHub** <br>

**Use a cloud based service or an IDE**<br>

**You can use one project for all exercises**<br>

**Exercise 3.0: Terminology** 
Copy and paste the contents of Part 3 in your README.md file.
``` 
.
.
.

## Part 3
<em>**What is Object Oriented Programming?**</em> - INSERT DEFINITION HERE <br>
<em>**Class inheritance**</em> - INSERT DEFINITION HERE <br>
<em>**What are getters and setters?**</em> - INSERT ANSWER HERE <br>
<em>**Difference between class variables and instance variables and class attributes?**</em> - INSERT ANSWER HERE <br>
<em>**What does self signify in a class?**</em> - INSERT ANSWER HERE <br>
<em>**Modules</em> - INSERT DEFINITION HERE <br>

## Part 4
```

- replace each <em>INSERT DEFINITION/ANSWER HERE</em> with the correct definition/answer in your own words. Using external resources are recommended.<br>

**Exercise 3.1: Basic class** <br>
Create a Ruby file called exercise-3.1.rb. 

1. Define a class called `Box`
2. Create three new `Box` instances.


Output 
```
> #<Box:0x00007fa5820e6508> 
> #<Box:0x00007fa58294a730> 
> #<Box:0x00007fa5850276c8> 
```

**Exercise 3.2: Animal class** <br>
Create a Ruby file called exercise-3.2.rb. 

1. Define a class called `Animal` and set attributes `name`, `animal_type` and `color` using the method attr_accessors (keep in mind, attributes refer to instance variables).
2. Initialize an Animal instance and store it in a variable called dog.
3. Access attributes `name` in dog and set it to "Clifford". Fill in the rest of the attributes.
4. Print out each attribute `dog` contains.
5. Create an instance method called `intro`. When you call `intro`, it should print `Hey, my name is Clifford. I'm red and I am a dog` to the console. Use string interpolation to do this.

Output 
```
> My name is Clifford. 
> I am a dog.
> My fur color is red.
```

**Exercise 3.3: Rectangle class** <br>
Create a Ruby file called exercise-3.3.rb. 

1. Define a class called `Rectangle` with instance variables `length` and `width`.
2. Define an instance method called `area`. This method should return the multiplication of `length` and `width`.
3. Define an instance method called `perimeter`. This should return the addition of all sides of the "rectangle". Refer to the mathematical formula below:
```
w + w + l + l
```
w refers to width 
l refers to length

**Exercise 3.4: Human class** <br>
Create a Ruby file called exercise-3.4.rb. 

1. Define a class called `Person` and set instance variables `name` and `age` using the method attr_accessors.
2. Define an initialize method that will set each attribute. 
3. Create a class variable called `people` that is set to an empty array.
4. Every time an instance gets created, push that instance in the class variable people. Do so in the initialize method.
5. Create a class method called `print_all_people`. Loop through people and print each name and age in the format of `"Name: John Doe, Age: 54"`. Call this method to see if the results are correct.

**Exercise 3.5: Class inheritance** <br>
Create a Ruby file called exercise-3.5.rb.

1. Define four classes: `Person`, `Doctor`, `Teacher` and `Engineer`. 
2. In the Person class, define an instance method called `eat` with a parameter called food. This method should print out "Eating " follow by the parameter. 
3. In `Person`, create attributes `weight`, `height`, `name`. 
4. In `Person`, define an initialize method and set these attributes by passing in arguments upon instantiation.
5. Make `Doctor`, `Teacher`, and `Engineer`inherit from `Person`.
6. For each class except Person, upon instantiation, print out "I am a " follow by the type of profession this person is in. 
For example, "I am a Doctor!".
7. Create a doctor instance, teacher instance, and engineer instance and check if they contain these attributes and methods inherited from the parent class `Person`.

**Exercise 3.6: Modules** <br>
Create a Ruby file called exercise-3.6.rb

1. Define a class called Person. 
2. Define a module called traits. In the module, define a method called eat and print out "Eating".
3. Include the module in the Person class. Allow each person instance to call these methods the module gives.


## Practice The Technical Interview 

<img src="https://assets.website-files.com/5f45dcafd2144b042ed84cfd/5f47ee151225c1378e7b9f6b_136_1588099272.png">

*Keep in mind, your skill level in solving algorithm challenges is separate from your skills in developing applications. In technical interviews, you may be told to solve these commonly used code challenges.*

**Exercise 3.7: Add Strings [leetcode](https://leetcode.com/problems/add-strings/)** <br> 
Create a Ruby file called exercise-3.7.rb

**I won't go easy on you...**

Given two non-negative integers, num1 and num2 represented as string, return the sum of num1 and num2 as a string.

You must solve the problem without using any built-in library for handling large integers (such as BigInteger). You must also not convert the inputs to integers directly.

Example 1: <br>

Input: num1 = "11", num2 = "123" <br>
Output: "134" <br>
Example 2: <br>

Input: num1 = "456", num2 = "77" <br>
Output: "533" <br>
Example 3: <br>

Input: num1 = "0", num2 = "0" <br>
Output: "0" <br>

**Exercise 3.8: Two Sum [leetcode](https://leetcode.com/problems/two-sum/)** <br> 
Create a Ruby file called exercise-3.8.rb

**Good job on the last question, let's see if you can figure this one out!**

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

Example 1:

Input: nums = [2,7,11,15], target = 9 <br>
Output: [0,1] <br>
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1]. <br>

Example 2: <br>

Input: nums = [3,2,4], target = 6 <br>
Output: [1,2] <br>

Example 3: <br>

Input: nums = [3,3], target = 6 <br>
Output: [0,1] <br>

**Exercise 3.9: Linked list** <br>
Create a Ruby file called exercise-3.9.rb

**You're tough if you made it this far.**

Create a linked list in Ruby.

Then, create a doubly linked list.

---

:wave: Saw a mispelled word? Want to improve the class exercises? Create a **pull request** and **contribute**! 
