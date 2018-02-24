---
title: "Loops"
lesson: 4
chapter: 1
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "tech"
type: "lesson"
tags:
    - programming
    - channels
    - for
    - loops
---

### Loops

For loops are the only looping structure in Go Lang but with it you can simulate any While, For While, etc loop.

Basic Syntax: 
`for <int>; <comparision>; <incremntor> { //code block } `

Example: 
``` Go
for i := 0; i < 5; i++ {
    // do something
}

for i > 16 {
    i++
}
```
any of the options for the For loop can be left off also.

##### Range 
the `range` command can be used with for to easily loop over arrays, lists, etc.