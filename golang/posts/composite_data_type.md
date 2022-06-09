### Composite data type
#### Arrays
- Fixed length series of elements of a chosen type
- Array literal: 
    - An array pre-defined with value
    - var x [5]int = [5]{1,2,3,4,5}
    - ... for size in array literal infers size from number of initializers
    - x:= [...]{1,2,3,4}

#### Iterating Through Arrays
- Use a for loop with `range` keyword
```
x:= [3]int {1,2,3}
for i, v range x {
    //do something
}
```
 
#### Slices
- A "window" on an underlying array
- Variable size, up to the whole array
