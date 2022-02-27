# Ruby Exercises - Part 4

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

## Part 4
<em>**Bundler**<em> - INSERT DEFINTION HERE <br>
<em>**Gemfile**<em> - INSERT DEFINITION HERE <br>
<em>**Bcrypt**<em> - INSERT DEFINITION HERE <br>
```

Project

**4.1 login + cli**
Create a Ruby file called exercise-4.1.rb

1. Copy and Paste the following

```ruby
require 'bundler/inline'
gemfile do
    source 'http://rubygems.org'
    gem 'bcrypt'
end
require 'bcrypt'

class User
    # Attributes
    attr_accessor :username, :password, :logged_in

    # Class Variables
    # Stores user instances
    @@users = []

    def initialize(username, password)
        @password = password
        @username = username
        @logged_in = false
        @@users << self
    end

    # Instance Methods
    # checks to see if the user is "logged in"
    def logged_in?
    end

    # salts password
    def create_hash_digest(password)
    end

    # Class Methods
    def self.all
        @@users
    end
        # "logs in user"
    def self.login(username, password)
    end
end

# Initializing instances
User.new("johndoe123", "password1")
User.new("skywoman456", "password2")
User.new("jimmyjohns789", "password3")


isLoggedIn = false

# Count to keep track of how many login attempts have been tried
tries = 0;

while (isLoggedIn == false)

    # Attempts
    tries += 1
    puts "Attempt #{tries} / 3"
    if(tries == 3)
        puts "Too many attempts, try again later"
        break;
    end
end
```

- Bundler has an inline gemfile definition feature that lets you define gem dependencies in a single-file Ruby script. To use this feature, require 'bundler/inline' and provide a gemfile block that has the code that you normally put in a Gemfile. This is done for you already.
- Take a second to digest the code here and understand it.
 
User Class,

1. In the `create_hash_digest` method, use BCrypt to hash the parameter `password`. Return it. 
2. In the `initialize` method, instead of `@password = password`, remove `password` and implement the `create_hash_digest` to hash the password.
3. In the `login` method, use the `each` method to iterate through `all` and check to see which user has the same username and password. If there is a match, set that user's `logged_in` attribute to true and then return the user. Otherwise, return nil.
4. In the `logged_in?` method, return the instance variable `logged_in`.

In the `while` Loop,

1. Print out "What is your username?". Get user input and store it in a variable called `username`. 
2. Then, print out "What is your password?". Get user input and store it in a variable called `password`.
3. Call the class method `login` from `User` and pass in `username` and `password` as arguments. 
4. `login` will return nil or the user, store whatever it returns in a variable called user. 
5. If the user exists (meaning if it is not nil) and is 'logged in', then print "Logged in succesful!" and then set `isLoggedIn` to true. This will stop the `while` loop.
6. Otherwise, increment `tries` and then print `Attempt #{tries} / 3`.

:wave: Saw a misspelled word? Want to improve the class exercises? Create a **pull request** and **contribute**!
