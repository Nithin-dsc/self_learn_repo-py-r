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

# Concatenate Elements:
  # You can also concatenate, or join, two or more elements, by using the paste() function.
   # To combine both text and a variable, R uses comma (,):

f <- 'awesome'
paste('R is',f) # "R is awesome"

# for numbers:
n1 <- 2
n2 <- 3
n3 <- n1 + n2
print(n3)

# Multiple Variables:
v1 <- v2 <- v3 <- 'fruit'
v1
v2
v3

### Basic Data types of R: ###
  # numeric - (10.5, 55, 787)
  # integer - (1L, 55L, 100L, where the letter "L" declares this as an integer)
  # complex - (9 + 3i, where "i" is the imaginary part)
  # character (a.k.a. string) - ("k", "R is exciting", "FALSE", "11.5")
  # logical (a.k.a. boolean) - (TRUE or FALSE)

# to check which variable,which types of datatype. we use class().

### Numbers ###
# numeric - (10.5, 55, 787)
# integer - (1L, 55L, 100L, where the letter "L" declares this as an integer)
# complex - (9 + 3i, where "i" is the imaginary part)

n = 8.6
i = 12L
c = 3i
class(n) 
class(i)
class(c)

 "numeric"
 "integer"
 "complex "

# Type conversion:
as.numeric()
as.integer()
as.complex()

# as.numeric():
as.numeric(i)
as.numeric(c)
# as.integer():
as.integer(n)
as.integer(c)
# as.complex():
as.complex(n) #  8.6+0i
as.complex(i) #  12+0i

# Math:
 # Math in numbers can be done by arthematic operations
x <- 5+5
x #10
# Moreover there are some built-in functions which help to do mathematical operations.

min(10,20,20) # 10
max(10,20,20) # 20
 # sqrt(): square root 
sqrt(16) # 4
sqrt(10) # 3.162278

# abs():
abs(-4) # 4
abs(3i) # 3
abs(-67.9i) # 67.9

# ceiling(): upward rounding.
ceiling(4.2) # 5

# floor(): backward rounding.
floor(4.2) # 4


                                                  ### Characters ###

# Character are strings: they need quoted with (' ') or ("") must.
char1 <- 'hello'

# Multiline characters:

multi_char = "Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."

print(multi_char) # "Lorem ipsum dolor sit amet,\nconsectetur adipiscing elit,\nsed do eiusmod tempor incididunt\nut labore et dolore magna aliqua."

# but for as it is like code:
cat(multi_char) 

#Lorem ipsum dolor sit amet,
#consectetur adipiscing elit,
#t labore et dolore magna aliqua.

# Combining two strings:

str1 <- 'Hello'
str2 <- 'world'
paste(str1,str2) # paste() function is used

## Escape characters:

str <- "We are the so-called "Vikings", from the north."
print(str) # error

str <- "We are the so-called \"Vikings\", from the north."
str # "We are the so-called \"Vikings\", from the north."
cat(str) # We are the so-called "Vikings", from the north.

# \n : for new line.
str ='We are the so-called "Vikings",\n from the north.'
str # "We are the so-called \"Vikings\",\n from the north."
cat(str) # We are the so-called "Vikings",
# from the north.

                                        ### Booleans: ###

5 < 6 # TRUE
9 > 19 # FALSE
10 == 10 # TRUE

# With if condition:
age <- 10
if (age == 18) {
  print('Eligible')
} else {
  print('Not Eligible')
}
 
           ### Operators: ###

# Arithmetic operators
# Assignment operators
# Comparison operators
# Logical operators
# Miscellaneous operators

## Arthematic Operators:
 # '+' additon
 # '-' subtraction
 # '/' division
 # '*' multiplication
 # '^' or '**'exponention
 # '%%' Modulus
 # '%/%' Round Division

## Assignment operators:

  # '<-' Leftward assignment  x <- 5
  # '=' Leftward assignment x = 5
  # '->' rightward assignment x -> 5
  # '<<-'	Global assignment (used in functions)	'x <<- 5'

## Comparisions operators:
  # ==	Equal to	5 == 3	FALSE
  # !=	Not equal to	5 != 3	TRUE
  # >	Greater than	5 > 3	TRUE
  # <	Less than	5 < 3	FALSE
  # >=	Greater than or equal to	5 >= 3	TRUE
  # <=	Less than or equal to	5 <= 3	FALSE

## Logical Operators:
 # &  - And (element wise)
 # |  - or  (element wise)
 # && - Logical And (in control flow)
 # || - LOgical Or  (in control flow)
 # !  - Not 

## The key difference between & and && (and | and ||) is that & and | are element-wise operators, meaning they operate on each element of a vector,
## while && and || only evaluate the first element of each vector. && and || are typically used for control flow (e.g., in if statements).

## Miscellaneous Operator:
 # ':' - Creates a series of numbers in a sequence	- x <- 1:10
 # %in% -	Find out if an element belongs to a vector -	x %in% y
 # %*% -	Matrix Multiplication	 -  x <- Matrix1 %*% Matrix2


            ### if...else ###
a <- 33
b <- 200

if (b>a){
  print(TRUE)
}else{
  print(FALSE)
}

# else if: similar elif in python.

if (b>a){
  print(TRUE)
}else if (a>b) {
  print(!FALSE)
}

# Nested if else:
x <- 41

if (x > 10) {
  print("Above ten")
  if (x > 20) {
    print("and also above 20!")
  } else {
    print("but not above 20.")
  }
} else {
  print("below 10.")
}

# with Logical:
a <- 200
b <- 33
c <- 500

if (a > b & c > a) {
  print("Both conditions are true")
}

 ### Exercise :

# 1 .Variable Assignment: Create three variables: name (character), age (numeric), and is_student (logical). 
# Assign appropriate values to them and print their values.

name = 'Nani'
age = 21
is_student = TRUE  

print(cat(name,age,is_student))

# 2. Arithmetic Operations: Calculate the area of a rectangle with length = 15 and width = 8.
#  Store the result in a variable called area and print it.

length = 15
width = 8
# a = wl
area = width * length
area # 120

# 3. Comparison Operators: Check if the age variable from exercise 1 is greater than or equal to 18. 
# Store the result in a variable called is_adult and print it.

age = 12
is_adult = TRUE
if (age >=  18) {
  is_adult <- TRUE
} else {
  is_adult <- FALSE }

print(is_adult)

# Logical Operators: You have two logical variables: has_license (TRUE if the person has a driver's license) and has_car (TRUE if the person owns a car). 
# Write an expression that evaluates to TRUE if the person has both a driver's license and a car.

has_license = FALSE
has_car = TRUE

if (has_license == TRUE & has_car == TRUE){
  print(TRUE)
}else{
  print(FALSE)
}
## Looping: 

i <- 6L
while (i>0){
  print(i)
  i = i - 1
}

# Break:
i <- 1
while (i < 6) {
  print(i)
  i <- i + 1
  if (i == 4) {
    break
  }
}

# next:
i <- 1
while (i < 10) {
  print(i)
  i <- i + 1
  if (i == 5) {
    next
  }
  print(i)
}
#  if..else in while loop.
dice <- 1
while (dice <= 6) {
  if (dice < 6) {
    print("No Yahtzee")
  } else {
    print("Yahtzee!")
  }
  dice <- dice + 1
}

# for looping:
x = 1:10
for(i in x){
  print(i)
}

for (i in 1:6){
  print(i)
} # op: 1 to 6 numbers(here 1,n-1 formula won't work)

fruits <- list("apple", "banana", "cherry")


                        ### Data Structure: ###

# R provides many built-in data structures. Each is used to handle data in different ways:
   
   # Vectors
   # Lists
   # Matrics
   # Arrays
   # Data frames
   # Factors



## Vectors:
  # A vector is the most basic data structure in R. It contains a list of items of the same type.
  # Vector - Single row of values - simple sequence.
  # To combine the list of items to a vector, use the c() function and separate the items by a comma.

fruits <- c('apple','banana','cherry','dragon fruit')
fruits

numbers <-c(1L,3L,'apple') 
numbers #"1"     "3"     "apple" (the vector converted data elements into single data type)

# Vector with numerical values in a sequence
numbers <- c(1:10)
numbers

decimals = c(1.0:5.6)
decimals # 1 2 3 4 5

decimals1 = c(1.2:6.2)
decimals1 # 1.2 2.2 3.2 4.2 5.2 6.2

# Vector of logical values
log_values <- c(TRUE, FALSE, TRUE, FALSE)
log_values

# lenght:
length(log_values) # 4

# sorting:
sort(log_values) # FALSE FALSE  TRUE  TRUE
fruits <- c("banana", "apple", "orange", "mango", "lemon")
sort(fruits) # "apple"  "banana" "orange"

# Accessing:
fruits[1] # banana (indexing starts from 1, not from 0 like pyhton)

# Accessing multiple items:
fruits[c(1:3)] # "banana" "apple"  "orange"
fruits[c(1,3,4)] #  "banana" "orange" "mango" 

# Accessing all items expect first item.
fruits[-1] #"apple"  "orange" "mango"  "lemon" 
fruits[c(-1)] # "apple"  "orange" "mango"  "lemon" 

# upadting or changing:
fruits[4] <- 'carrot'
fruits # "banana" "apple"  "orange" "carrot" "lemon" 

# repeat vectors 'rep()':

repeat_vectors <- rep(c(1,2,3),4)
repeat_vectors # 1 2 3 1 2 3 1 2 3 1 2 3

# Sequence Vectors seq():
sequence_vectors <- seq(1,9)  # 1 2 3 4 5 6 7 8 9
sequence_vectors2 <- c(1:9) # 1 2 3 4 5 6 7 8 9
 ## Creating a sequence from 1 to 10 with a step of 3
sequence_vectors3  <- seq(1,10,by = 3) # 1 4 7 10

# Logical Indexing:
numeric_vector <-c(seq(1,30,by = 2))
greater_than_15 <- numeric_vector[numeric_vector > 15]
print(greater_than_15)

# Selecting elements equal to 10 or 20
equal_10_or_20 <- numeric_vector[numeric_vector == 10 | numeric_vector == 20]
equal_10_or_20 # numeric(0) no elements 


# Vectore Operations:

vector1 = c(1:5)
vector2 = c(6:10)
vector3 = vector1 + vector2
vector3 # 7  9 11 13 15

# Subtraction
subtraction <- vector2 - vector1
print(subtraction)

# we do all operation:

# Recycled vector:

vector3 <- c(1, 2)
vector4 <- c(3, 4, 5, 6)

recycled_vector = vector3 + vector4
recycled_vector # warning both are not same lenght.

# Logical Operations:
log1 = vector1 & vector2
log1  # TRUE TRUE TRUE TRUE TRUE

log2 = vector3 & vector4
log2

## Using built-in functions:

sqrt(vector1) #  1.000000 1.414214 1.732051 2.000000 2.236068

abs(vector1) #  1 2 3 4 5

logarithms <- log(vector1)
logarithms # 0.0000000 0.6931472 1.0986123 1.3862944 1.6094379

vector_with_duplicates <- c(1, 2, 2, 3, 4, 4, 5)
print(unique(vector_with_duplicates)) # 1 2 3 4 5

## Practice Activities:

## 1.Create a vector named temperatures containing the following values: 22, 25, 28, 27, 24, 23, 26.
#  These represent daily temperatures in Celsius.
# Calculate the average temperature.
# Find the days where the temperature was above 25 degrees Celsius using logical indexing.
# Convert the temperatures to Fahrenheit using the formula: F = (C * 9/5) + 32.

temperatures <- c(22, 25, 28, 27, 24, 23, 26)
average = sum(temperatures)/ length(temperatures)
average # 25

temp_25 =  temperatures[temperatures>25]
print(temp_25) # 28 27 26

Fahrenheit = ( temperatures * 9/5 + 32)
Fahrenheit # 71.6 77.0 82.4 80.6 75.2 73.4 78.8

#2. Create two character vectors:
# Fruits <- c("apple", "banana", "orange")
# Veggies <- c("carrot", "broccoli", "spinach") 
# Combine these two vectors into a single vector called produce.
# Add "mango" to the beginning, and "peas" to the end of produce.

Fruits <- c("apple", "banana", "orange")
Veggies <- c("carrot", "broccoli", "spinach") 
produce = c(Veggies,Fruits) # "carrot"   "broccoli" "spinach"  "apple"    "banana"   "orange"  

produce[1]<- 'mango'
produce[length(produce)]<- 'peas'
print(produce) # "mango"    "broccoli" "spinach"  "apple"    "banana"   "peas"    
# or
produce = c('peas',produce,'mango')
produce # "peas"     "mango"    "broccoli" "spinach"  "apple"    "banana"   "peas"     "mango"   
unique(produce) # "peas"     "mango"    "broccoli" "spinach"  "apple"    "banana"  

#3. Given the vector numbers <- c(5, 10, 15, 20, 5, 25, 10):
# Find the unique values in the numbers vector.
# Count how many times the value 5 appears in the original numbers vector.
numbers <- c(5, 10, 15, 20, 5, 25, 10)
unq_values = unique(numbers)
unq_values

# counting 5 in numbers
count_of_5 = sum(numbers==5)
print(count_of_5) # 2

# 4. Create a vector of even numbers from 2 to 20 using the seq() function.
# Then, create a vector of odd numbers from 1 to 19.
# Multiply each even number by its corresponding odd number (element-wise).

even_numbers <- seq(2,20,by=2)
odd_numbers <- seq(1,19,by = 2)
print(even_numbers*odd_numbers)



