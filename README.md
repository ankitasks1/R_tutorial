#  R_tutorial

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

