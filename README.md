#  R_tutorial
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

<code>
library(data.table)
dt <- fread("data.txt", header =T)
</code>
