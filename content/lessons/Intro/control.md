---
title: "Control Commands"
lesson: 6
chapter: 1
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "Intro"
type: "lesson"
tags:
    - programming
    - if
    - else
    - loop
    - switch
---

### Control Structors (if/else/switch)

#### if command

#### switch
Syntax: 
```
    switch <variable> {
        case <value>:
            // some code
        case <value2> 
            // some other code
        default: 
            // some code that runs if the others do not.
    }
```

the switch command allows one of many conditionals to be selected based on the "switch".  In the simple and probably most commong example switch command takes a single parameter and based on it does one of many cases.

simple example: 
``` go
 	

    i := 2
    fmt.Print("Write ", i, " as ")
    switch i {
    case 1:
        fmt.Println("one")
    case 2:
        fmt.Println("two")
    case 3:
        fmt.Println("three")
    }

```

example: (from: https://gobyexample.com/switch)
``` go
switch time.Now().Weekday() {
    case time.Saturday, time.Sunday:
        fmt.Println("It's the weekend")
    default:
        fmt.Println("It's a weekday")
    }
```
