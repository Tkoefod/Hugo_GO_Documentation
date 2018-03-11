---
title: "Slices"
lesson: 2
---

1. single type
2. numbered sequence 

slices are typed only by the elements they contain (not the number of elements).

### Declare new Slice
    ie: `s := make([]string, 3)`
makes a new slice of array string type length 3 with inital values of 0

### assigning values
```go
    s[0] = "something1"
    s[1] = "something2"
    s[2] = "c"
```
assign values to already created slices.

### built in methods for slices

#### append
newslice = append(origSlice, newValue, newValue2)
```go
    s = append(s, "something4")
    s = append(s, "sometthing5", "f")
```

#### copy
copy(fromSlice, toSlice)