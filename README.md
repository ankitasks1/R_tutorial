#  R_tutorial

## Setting directory where you want to work
```
setwd("directory")
eg.
setwd("/Archive2/home/")
```
## Getting directory where you are working
```
getwd()
```

## Install packages
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

## Input
### Assignment
```
vec <- c(3,5,7,9)
```

## Reading file
```
dt <- read.table("data.txt", header =T) 
dt <- read.csv("data.csv", header=T)
```

or

```
library(data.table)
dt <- fread("data.txt", header =T)
```

## Listing environment
```
ls()
```

## Remove an object
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
length(df)
hist() #histogram
q() #quit n close R session			
rm(list = ls())#remove all files in listed directory
list.files()
.libPaths()		# library pathname
.Library	# library pathname
ncol(df)
nrow(df)
dim(df)
names(df)
colnames(df)
rownames(df)
class(df)
duplicated(df$col)
which()
## Basic stattistic function
max()
min()
mean()
median()
sd()
lm()

#For Plotting
plot(density(df$col, na.rm=TRUE))				

par(ask=TRUE) #One figure in frame
par(mfrow=c(2,3)) # 6 figures in one frame 2 rows 3 columns
plot()
plot(density())
boxplot()
stripchart()
qqnorm()
barplot()

sessionInfo()

#Want to write your own functions? Learn here
https://www.dataquest.io/blog/write-functions-in-r/

