# self_learn_repo-py-r
Self learn repo for python and R language
# new file for r language 
a = 1
b = 2
c = a+b

#  Assigning a value to a variable
x <- 5
x

# Printing text
print("Hello, R!")

# Get Working Directory: Use the getwd() function to get the current working directory.
getwd() # "C:/Users/yempa"

# Set Working Directory: Use the setwd() function to set the working directory.
setwd() # used to set directory 
## setwd("/path/to/your/directory")  # Replace with your actual directory path

# Installing and Loading Packages
  ## R's functionality can be extended through packages. To use a package, you first need to install it, 
    # and then load it into your R session.

install.packages("ggplot2")

# Load package: with library() function.
library(ggplot2)
 ## In r we need to install package once, but need to load every time when function are used from package.

# Basic syntax and conventions: conventions that you need to understand to write effective code.
 # R is also case-sensitive like python, here x and X is not similar.
 # Moreover, naming conventions are also same.

## Statements and Expressions:
  # Statments:statement is a complete instruction that the interpreter can execute.
  # Expression: is a part of a statement that can be evaluated to produce a value.

x <- 10 # statment
x*2 # expression

# Variables and Assignment:
myvar = 12
myVar = 13
MyVar = myvar + myVar

# Style's of R:
  # Google's R Style Guide: Focuses on consistency and readability.
  # Tidyverse Style Guide: Emphasizes using the tidyverse packages and their conventions.

## Key aspects of code style:
 # indentation: Use consistent indentation (usually 2 or 4 spaces) to indicate code blocks.
 # pacing: Use spaces around operators (e.g., x <- 1 + 2) and after commas (e.g., my_function(arg1, arg2)).
 # Line Length: Keep lines reasonably short (e.g., 80 characters) to avoid horizontal scrolling.
 # Naming Conventions: Use descriptive variable and function names. Consider using snake_case (e.g., my_variable_name) for variables and functions.

# ouput variable:
c = 12
c 
print(c)

