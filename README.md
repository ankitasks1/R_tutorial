#  R_tutorial
## Input
### Assignment
<code>
vec <- c(3,5,7,9)
</code>

## Reading file
<code>
dt <- read.table("data.txt", header =T)
dt <- read.csv("data.csv", header=T)

or

library(data.table)
dt <- fread("data.txt", header =T)

</code>
