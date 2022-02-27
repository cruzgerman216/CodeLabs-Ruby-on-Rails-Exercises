# Ruby - Command Line Interface Project

## READ BEFORE STARTING

**Use a cloud based service or a local IDE**<br>

**Create a GitHub Repository/commit frequently**<br>


You've gone through Ruby syntax and most importantly programming fundamentals. That should be enough to create an awesome Ruby CLI, a command line interface. 

## Setup 
```bundle gem project_name` to create a gem. Use the directory/file structure to your advantage to organize files. 

### bin/run 
Under bin, create a file called `run`. Use the shebang line ```#!/usr/bin/env ruby ``` at the top of your file. Now if you enter `bin/run` in the terminal, it should execute `run` as a ruby file. 

In case you get a `permission denied` error, run `chmod +x bin/*`.

### README.md 
Create a `README.md` file in the root directory of the project.

Copy and paste: 
```
# TODO: Enter project name 

TODO: Add project summary
```

Fufill each todo. 

## Requirements 
You can code anything in this project as long as it meets the requirements: 

- Get user input and display output/info
- Project Theme examples but not limited to the following:
  - text adventure game 
  - scrape data from a webpage/display info
  - create a utility your computer doesn't have
- Menu
  - A menu is a series of options the user can choose from. 

#### Optional 
- Scrape data using Nokogiri/open-uri
- Incorporate a login/logout system using BCrypt
- Send requests to an API to capture data
- Publish your Gem to `RubyGems`