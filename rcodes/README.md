# R Codebook
Below are codes we have used in class or homework that will be useful to keep in mind.  

## Lecture 2

?<'function-name'> | Will load the help for any built in function or any library function which has been properly documented. 

cat "quote" | Presents a series of words without trying to run as code.

'+' '-' '*' '/' 'pi' 'sin()' | Algebraic Functions

<- = | Assignment Functions

<<- | Permanent Assignment Function

; | Statement seperator, allows multiple command in one line.

'c(<variable/values>)' '1:10' | Produces an array of the values.

'if () {} else {}' | Conditionals

'while () {}' 'for () {}' | Loops

### library(tidyverse) commands

read_csv | Reads in the dataset you want to use.

head 'value' | Prints out the number of rows from the dataset you want to see. For entire set, just use 'head'.

%>% | Pipe Operator in tidyverse that passes the output of one function as the input to the next.

### library(dplyr)

group_by('var') | Determines how you want your data grouped by when you print out using 'head'

tally() | A shortcut for counting rows in each group of a data frame.

arrange(desc(n)) | Arranges values in a descending order

'column_names' <- 'var' | Allows you to select a column to control based on its name  




sprintf("text") | Formats variables based on type and assigns them a scripted quote  
  
%s | string, %d | integer, %.2f | 2 decimal places, \n | new line, \t | tab  
  
