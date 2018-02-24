---
title: "Wait Groups"
lesson: 4
chapter: 3
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "tech"
type: "lesson"
tags:
    - programming
    - channels
    - concurrency
    - waitgroup
    - wg
---

### the convience of Wait Groups


#### iterating over channels

example:

```
package main

import (
  "fmt"
  "sync"
  )

var wg sync.WaitGroup

func foo(c chan int, someValue int){
  defer wg.Done()
  c <- someValue * 5
}

func main() {
  fooVal := make(chan int, 10)
  for i := 0; i < 10 ; i++ {
    wg.Add(1)
      go foo(fooVal, i)
  }
  wg.Wait()
  close(fooVal)

  for item := range fooVal {
    fmt.Println(item)
  }
}
```
