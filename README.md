#  R_tutorial
R is a programming language and software environment for statistical computing and graphics. It's used for a wide range of tasks, including data analysis, visualization, statistical modeling, and machine learning. R is also known for its extensibility and flexibility. 

### Object types in R

#### String (Character Vector) – Text data
```
my_string <- "Hello Team"  # character vector of length 1
```

##### Vector – Basic 1D structure (same type)
```
my_vector <- c(1, 2, 3, 4)  # numeric vector
```

#### List – Collection of elements (can be different types)
```
my_list <- list(name = "Alice", age = 30, scores = c(85, 90))  # mixed types
```

#### Data Frame – Table-like structure (columns can be different types)
```
my_df <- data.frame(name = c("Alice", "Bob"), age = c(30, 25))  # like a spreadsheet
```

#### Matrix – 2D structure (all elements must be same type)
```
my_matrix <- matrix(1:6, nrow = 2, ncol = 3)  # numeric matrix
```

#### Array – Multi-dimensional structure
```
my_array <- array(1:8, dim = c(2, 2, 2))  # 3D numeric array
```

#### Factor – Categorical variable (used for groupings, labels)
```
my_factor <- factor(c("yes", "no", "yes", "no"))  # stores "levels"
```

#### Tibble – Modern data frame (from tidyverse)
```
library(tibble)
my_tibble <- tibble(name = c("Alice", "Bob"), score = c(90, 85))  # tidy format
```

#### Functions
```
my_function <- function(x) {
  return(x + 1)
}
my_function(4)  # returns 5
```

### Basic Data Types
```
numeric - (10.5, 55, 787)
integer - (1L, 55L, 100L, where the letter "L" declares this as an integer)
complex - (9 + 3i, where "i" is the imaginary part)
character (a.k.a. string) - ("k", "R is exciting", "FALSE", "11.5")
logical (a.k.a. boolean) - (TRUE or FALSE)
```


### Setting directory where you want to work
```
setwd("directory")
eg.
setwd("/Archive2/home/")
```
### Getting directory where you are working
```
getwd()
```

### Install packages
##### CRAN
```
install.packages("package")
```

##### BiocManager
```
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("DESeq2")
```

### Load package
```
library(package)
```

### Load package manual help
```
help(package=package)
```

### Getting Inputs
#### Assignment
```
vec <- c(3,5,7,9)
```

### Reading file
```
dt <- read.table("data.txt", header =T) 
dt <- read.csv("data.csv", header=T)
```

or

```
library(data.table)
dt <- fread("data.txt", header =T)
```

### Listing environment and files
```
ls()
list.files()
```

### Remove an object
```
rm(df)
```

### Attach Set of R Objects to Search Path
```
attach(df)
```

### Identify data structure
```
str(df)
```
### Show the top lines
```
head(df,3) 
```

### Show the last lines
```
tail(df,3) 
```

### Rounding off
```
round(2.9010, 2)
```

### Summarize dataframe
```
summary(df)
```

### Select specific row
```
which()
```

### length and dimensions 
```
length(df$column)
dim(df)
```

### R libraries pathname
```
.libPaths()		
```

### number of columns and rows in a dataframe
```
ncol(df)
nrow(df)
```

names(list)

### column names
```
colnames(df)
```

### row names
```
rownames(df)
```

### type of data
class(df)

### get duplicates
duplicated(df$col)

### Basic stattistic function
```
max(vec)
min(vec)
mean(vec)
median(vec)
sd(vec)
```
### For Plotting
#### histogram
```
hist(vec) 
```
#### density distribution
```
plot(density(df$col, na.rm=TRUE))
par(ask=TRUE) #One figure in frame
par(mfrow=c(2,3)) # 6 figures in one frame 2 rows 3 columns
```

#### boxplot
```
boxplot()
```

#### barplot
```
barplot()
```

#### plotting with ggplot2
```
ggplot(data=iris, aes(x=Species, y=Sepal.Length)) +  geom_bar(stat="identity", fill="#2596be", width=0.4)

![plot](https://raw.githubusercontent.com/ankitasks1/R_tutorial/main/Rplot.png)
```

  
### Session info
```
sessionInfo()
```

#### training datasets 
```
library(mtcars)
library(iris)
```
#### Want to write your own functions? Learn here
https://www.dataquest.io/blog/write-functions-in-r/

