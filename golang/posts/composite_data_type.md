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

#### Hash table
- Contain key/value pairs
- Hash function is used to compute the slot for a key
- Advantages:
  - Fast lookup than lists
    - Constants time, vs. linear time
  - Arbitrary keys
    - Not ints, like slices or array
- Disadvantage:
  - May have collision: two keys hash to same slot

#### Map
- Implementation of a hash table
- Use make() to create a map

#### Structs