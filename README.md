# My-R-Notes
## Notes for R Programming Coursera
### [Coercion] (http://adv-r.had.co.nz/Data-structures.html)

Link: http://adv-r.had.co.nz/Data-structures.html

* Given a vector, you can determine its type with typeof(), or check if it’s a specific type 
with an “is” function: is.character(), is.double(), is.integer(), is.logical(), or, more generally, is.atomic().

  int_var <- c(1L, 6L, 10L)
  
  typeof(int_var)
  
  #> [1] "integer"
  
  is.integer(int_var)
  #> [1] TRUE  
  is.atomic(int_var)
  #> [1] TRUE

* All elements of an atomic vector must be the same type, so when you attempt to combine different types they will be coerced to the most flexible type. 
Types from least to most flexible are: logical, integer, double, and character. 
