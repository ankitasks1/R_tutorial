#  R_tutorial

## setting directory where you want to work
```
setwd("directory")
eg.
setwd("/Archive2/home/")
```
## getting directory where you are working
```
getwd()
```

## Input
### Assignment
```
vec <- c(3,5,7,9)
```

## Reading file
```
dt <- read.table("data.txt", header =T) # read.table part of base function R: utils
dt <- read.csv("data.csv", header=T) # read.csv part of base function R: utils
```

or

```
library(data.table)
dt <- fread("data.txt", header =T)
```

## list
```
ls()
```

## remove an object
```
rm()
```
	
plot(density(df$col, na.rm=TRUE))				
install.packages("package")				
library(package)
help(package=package)
sessionInfo()
attach(df)
str(df) #Identify structure
head(df,3) # Show the head 3 lines
tail(df,3) # Show the last 3 lines
round()
summary(df)
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
max()
min()
mean()
sd()
#For Plotting
par(ask=TRUE) #One figure in frame
par(mfrow=c(2,3)) # 6 figures in one frame 2 rows 3 columns
plot()
plot(density())
boxplot()
stripchart()
qqnorm()
barplot()


#Want to write your own functions? Learn here
https://www.dataquest.io/blog/write-functions-in-r/

