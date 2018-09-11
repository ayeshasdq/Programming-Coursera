# Programming-Coursera
Coursera Assignment# 2: Programming

#matrix can be created after calling a makeCacheMatrix without arguments.

# read the R script

# call makeCacheMatrix without arguments
a <- makeCacheMatrix();
summary(a);
#>              Length Class  Mode    
#> setMatrix    1      -none- function
#> getMatrix    1      -none- function
#> cacheInverse 1      -none- function
#> getInverse   1      -none- function

# create a square matrix (reason `solve` only handles square matrices )
a$setMatrix( matrix(c(1,2,12,13), nrow = 2, ncol = 2) );
a$getMatrix();


cacheSolve(a)

# the 2nd time we run the function, we get the cached value
cacheSolve(a)
#> getting cached data
