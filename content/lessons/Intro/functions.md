---
title: "Functions"
lesson: 5
chapter: 1
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "tech"
type: "lesson"
tags:
    - programming
    - functions
---

### Functions

functions in go not only can take multiple arguments but can also return multiple values.

Define a Function:
` func <funcname>( <in Variables> ) <out variable types>  { // so somehting }`

_example:_ 
``` Go
func myFunction( passedParam string ) int {

}
```

#### Variadic Functions
Functions that take a variable amount of arguments

```go
func sum(nums ...int) {
    fmt.Print(nums, " ")
    total := 0
    for _, num := range nums {
        total += num
    }
    fmt.Println(total)
}
```