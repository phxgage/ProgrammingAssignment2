ProgrammingAssignment2
======================

Repository for Programming Assignment 2 for R Programming on Coursera

---
title: "README.md"
author: "J O Smith (phxgage)"
date: "July 10, 2014"
output: html_document
---

# SOLUTION TO PROGRAMMING ASSIGNMENT 2
## Approach
* Follow general outline of example in assignment
* Use CAPITAL Letters for external matrix variables
* Use lower case letters for interal matrix variable
* Differentiate between internal/EXTERNAL variables with variable case
** inv: internal inverse variable
** INV: external inverse variable

## Notes:
* Sample Output formatting fixed 7/10/14

## Sample Output
```
> a <- c(1,2,3,4)
> dim(a) <- c(2,2)
> a
     [,1] [,2]
 [1,]    1    3
 [2,]    2    4
> class(a)
[1] "matrix"
> A <- makeCacheMatrix(a)
> A$get()
     [,1] [,2]
[1,]    1    3
[2,]    2    4
> A$getinv()
NULL
> V <- cacheSolve(A)
> V
     [,1] [,2]
[1,]   -2  1.5
[2,]    1 -0.5
> A$getinv()
     [,1] [,2]
[1,]   -2  1.5
[2,]    1 -0.5
> Ainv <- A$getinv()
> A0 <- A$get()
> A0 %*% Ainv
     [,1] [,2]
[1,]    1    0
[2,]    0    1
```
