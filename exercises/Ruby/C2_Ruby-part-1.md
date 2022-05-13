# Ruby Exercises - Part 1

## READ BEFORE STARTING

**Use Git or GitHub Desktop to commit each exercise to GitHub** <br>

**Use a cloud based service or an IDE**<br>

**You can use one project for all exercises**<br>

**Exercise 0: Setup** 
- Create a folder called Code-Labs-Ruby-Exercises. Publish this to GitHub and name the repo `Code-Labs-Ruby-Exercises`. Create four separate folders: part-1-exercises, part-2-exercises, part-3-exercises, part-4-exercises. When ask to create a file, store them in the appropriate folders. 
- Create a **README.md** file at the root directory. In your README.md file. Copy and paste the following: 

``` 
# Ruby Exercises and Terminology 
[Link to exercises](https://github.com/cruzgerman216/CodeLabs-Ruby-on-Rails-Exercises) <br>
Here is a list of ruby terms and definitions used in class.

## Part 1 
<em>**Layer of Abstraction**</em> - INSERT DEFINITION HERE <br>
<em>**Data Type**</em> - INSERT DEFINITION HERE <br>
<em>**Variable**</em> - INSERT DEFINITION HERE <br>
<em>**What's the difference between a local variable, constant variable, and a global variable?**</em> - INSERT DEFINITION HERE <br>
<em>**What does scope mean?**</em> - INSERT DEFINITION HERE <br>
<em>**Constant Variable**</em> - INSERT DEFINITION HERE <br>
<em>**Method**</em> - INSERT DEFINITION HERE <br>
<em>**IRB**</em> - INSERT DEFINITION HERE <br>
<em>**Operators**</em> - INSERT DEFINITION HERE <br>
<em>**Class**</em> - INSERT DEFINITION HERE <br>
<em>**Gem**</em> - INSERT DEFINITION HERE <br>

## Part 2

## Part 3

## Part 4
```

- replace each <em>INSERT DEFINITION HERE</em> with the correct definition in your own words. Using external resources are recommended.<br>

**Exercise 1.1: Print to the console** <br>
Create a ruby file called exercise-1.1.rb. 
- Use the method p to print out the string `p` to the console
- Use the method puts to print out the string `puts` to the console
- Use the method print to print out the string `print` to the console
- Create a variable called my_name and set it to your name. Print it to the console.
- Create a variable called beginning_sentence and set it to `My name is `. Create another variable called full_sentence and set it equal to the combination of both beginning_sentence and my_name. Use the `+` operator to do that. Print full_sentence. 

Result: 

``` 
> "p"
> puts
> printMy name is German
```
**Exercise 1.2: Define a method** <br>
Create a ruby file called exercise-1.2.rb. 
- Define a method called say_hello_to. When you call the method, you should be able to see `Hello, John Doe!` in the console.
- Add a parameter called name to the method you just created. Use the parameter to print out `Hello, ` follow by the parameter name. Use string interpolation to do this.
- Create a constant variable called my_name and set to your name.
- Call the method and add the my_name variable as an argument.

Result: 
```
> Hello, German
```

**Exercise 1.3: Multiple Methods** <br>
Create a ruby file called exercise-1.3.rb. Copy and paste the following:

```ruby

def favorite_movie(movie)
    # TODO: use string interpolation to print "My favorite movie is " and include the movie parameter.
end

def favorite_food(food)
    # TODO: use string interpolation to print "My favorite food is " and include the food parameter.
end

def favorite_drink(drink)
    # TODO: use string interpolation to print "My favorite drink is " and include the drink parameter.
end 

def list_of_favorite_things(movie, food, drink)
    # TODO: Call favorite_movie, pass in the parameter movie as an argument
    # TODO: Call favorite_food, pass in the parameter food as an argument 
    # TODO: Call favorite_drink, pass in the parameter drink as an argument 

end

# TODO: Call list_of_favorite_things, include three arguments
```

- Read each comment and complete each task.

Result: 
```
> My favorite movie is The Thing
> My favorite food is spaghetti
> My favorite drink is water
```

**Exercise 1.4: Define a method with multiple arguments** <br>
Create a ruby file called exercise-1.4.rb. 

- Define a method called names_of_my_pets. Add three parameters to the method: name_1, name_2, name_3.
- Create three variables that correspond to the parameters of your method. Set them to whatever value you like.
- When calling the method, be should to pass in these variables as arguments. Here is the expect result:

Result: 
```
> I have 3 pets! Their names are Apollo, Athena and Loki!
```

**Exercise 1.5: Use built in string methods** <br>
Create a ruby file called exercise-1.5.rb. 

- Create a variable called sentence and set it to `Hello John Doe!`. Use the built-in string method `sub` to replace `Hello` with `Hi`. If you don't know how to use `sub`, I suggest Googling it. Print out the result. 
- Create a variable called solution and set it to `Hi John Doe!`. Use the built-in string method `match?`to check your output from the previous problem. Print the result and you should get `true` in the console.

Result:
``` 
> Hi John Doe!
> true
```

**Exercise 1.6: Use escaping to output single quotes in a string** <br>
Create a ruby file called exercise-1.6.rb. 

- Output `'Single Quotes' is actually my favorite movie. It's great.` to the console (hint: backslashes)

**Exercise 1.7: Print out user input** <br>
Create a ruby file called exercise-1.7.rb. 

- Use `gets.chomp` to get the user input, then store it in a variable called user_input. Print into the console "You typed: " follow by what the user entered.
- Define a method named multiply_by_two with one parameter. Get the user input and use the method you defined to multiply that number by 2. Print the result.
- Define a method named divide_by_two with one parameter. Take in a user input and store and divide that value by two using divided_by_two. Print the result.

Result:
```
> Please enter a sentence: 
> I enjoy coding!
> You have typed 'I enjoy coding!'
> What number do you want to multiply by two?
> 5
> 5 multiplied by 2 is 10
> What number do you want to divide by two?
> 10
> 10 divided by 2 is 5
```

**Exercise 1.8: Built in String methods** <br>
Create a ruby file called exercise-1.8.rb. 
Go through the [ruby documentation](https://ruby-doc.org/core-3.1.0/String.html#method-i-next). Use 5 built in string methods. Here's an example of using the string method `length`.

```ruby
name = "John"
puts "I have #{name.length} characters in my name."
```

**Exercise 1.9: Operators**<br>
Create a ruby file called exercise-1.9.rb

Create four methods: add, subtract, divide and multiply. Each method should have two parameters. Each method should do a basic level of an expression involving a certain operator and the given two parameters. For example, in the `add` method, you will use the `+` to evaluate the addition of both parameters. 

:wave: Saw a misspelled word? Want to improve the class exercises? Create a **pull request** and **contribute**! 