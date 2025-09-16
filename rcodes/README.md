# R Codebook
Below are codes we have used in class or homework that will be useful to keep in mind.  

## Lecture 2 - tidyverse, dplyr

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

getwd() | Recognizes all files within the working directory.

'df' <- read_csv | Reads in the dataset you want to use.

head('df','value') | Prints out the number of rows from the dataset you want to see. For entire set, just use 'head'.

%>% | Pipe Operator in tidyverse that passes the output of one function as the input to the next.

### library(dplyr)

group_by('var') | Determines how you want your data grouped by when you print out using 'head'

tally() | A shortcut for counting rows in each group of a data frame.

arrange(desc(n)) | Arranges values in a descending order

summarize(name=expr,...) | operate per group and produce a table of summaries

'column_names' <- 'var' | Allows you to select a column to control based on its name  

tibble | a more efficient data frame class (like table)

select(c1,c2,...) | returns a new data frame with only the selected columns

rename(new_name=old_name, ...) | return a new data frame with the renamings

mutate(name=expr,...) | adds or modifies columns

filter(boolean_expr) | returns a dataframe with only matching rows

## Lecture 4 - ggplot

readr | loads a file into a data frame

### library(ggplot2)

ggplot | tidyverse plot function; works by letting you associate data with aesthetics; chains with +

geom_point | points

geom_histogram | histogram, performs aggregation itself (geom_bar + stat bin)

geom_density | density plot (using a kernel density estimate)

geom_boxplot | boxplot (plots centroids and widths w/ outliers)

geom_rect | general rectangles

geom_bar | bar graph can perform all sorts of aggregations

aes() | how variables in your dataset should be mapped to visual properties of the plot 

color | the color of a point or shape or the color of the boundary of a polygon or rectangle 

fill | the color of the interior of a polygon or rectangle 

alpha | the transparency of a color 

position | for histograms and bar plots how to position boxes for the same x aesthetic. "dodge" is the most clear.  

## Lecture 5 - pivots and joins

'new_df' <- pivot_longer | Fixed table so that names are moved to their own column and observations are what is put in the column field.

left_join('function') | Moves data from a secondary dataset into the first by merging column names, may require renaming.

inner_join('function') | Creates a new dataset that only has the homogenous data between the two

right_join('function') Moves data from a primary dataset into the second by mergining column names.

full_join('function') | Combines all data between two sets within a table

semi_join('var', by...) | returns only the rows from the left table that have a match in the right table, without adding columns

anti_join('var', by...) | returns only the rows from the left table that do not have a match in the right table.

joining lookups | using a table of reference values to add descriptive information or labels to another table based on a key.

chaining joins | performing multiple joins sequentially to combine more than two tables step by step.

## Lecture 6

names('df') | Displays all names in the dataset

sort(decreasing = T) %>% names() | Sort the counts of shapes in descending order and get the names.

sprintf("text") | Formats variables based on type and assigns them a scripted quote  

%s | string, %d | integer, %.2f | 2 decimal places, \n | new line, \t | tab |

as.Date('var', format ='var format') = Change a variable into a date format (YYYY/MM/DD)

gsub('Old obs','New obs','df$var') = Substitutes one value for another inside of a dataset

setdiff('x','y') | Reads in obs for x but not for y
