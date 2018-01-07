## Pascal triangle
- Print as below:  
```
     1  
    1 1  
   1 2 1  
  1 3 3 1  
 1 4 6 4 1  
```
- Given col and row (start from 0), get the element's value by means of recursive process.
*Note* Two points need to be addressed: 1. Termination condition, 2. Recursive call
```scala
def pascal(c:Int,r:Int):Int= if(c==0 || r==0 || c==r) 1 else pascal(c-1,r-1) + pascal(c,r-1)

for (row <- 0 to n) {
  0 to (n - row) foreach { _ => print(" ") }
  for (col <- 0 to row) {
    print(pascal(col, row) + " ")
  }
  println()
}

```


