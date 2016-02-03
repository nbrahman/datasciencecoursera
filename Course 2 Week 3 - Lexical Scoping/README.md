##Course 2 Week 3 - Lexical Scoping

In this project, we were needed to write an R function that is able to cache potentially time-consuming computations. For example, taking the mean of a numeric vector is typically a fast operation. However, for a very long vector, it may take too long to compute the mean, especially if it has to be computed repeatedly (e.g. in a loop). If the contents of a vector are not changing, it may make sense to cache the value of the mean so that when we need it again, it can be looked up in the cache rather than recomputed. In this Programming Assignment will take advantage of the scoping rules of the R language and how they can be manipulated to preserve state inside of an R object.

###Caching the Inverse of a Matrix

Matrix inversion is usually a costly computation and there may be some benefit to caching the inverse of a matrix rather than compute it repeatedly.

Following two functions were written to complete the project requirements

**1. makeCacheMatrix:** This function creates a special "matrix" object that can cache its inverse.

**2. cacheSolve:** This function computes the inverse of the special "matrix" returned by makeCacheMatrix above. If the inverse has already been calculated (and the matrix has not changed), then the cachesolve will retrieve the inverse from the cache.

Computing the inverse of a square matrix is done with the '**solve**' function in R.

The R source code includes the appropriate code to validate the arguments passed to all the functions along with the validation if the passed matrix is actually reversible.
