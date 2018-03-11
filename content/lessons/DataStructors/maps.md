---
title: "Maps"
lesson: 3
---

built-in associative data type (aka known as hashes or dicts in other languages).
	

### create a map
` m := make(map[string]int) `
makes map 'm' with key type 'string' and value type 'int'
example: 
```go
    m := make(map[string]int)
    m["one"] = 17
    m["two"] = 02
    valueOne := m["one"]
```

maps are unsorted set of data consisting of keys and values that are associated to them.  If you ask to get the value of a key that doesn't exist '0' is returned.

| Action | Example |
| ---  | ---     |
| create emptry map |  `m := make(map[string]int)` |
| create & declare  | `n := map[string]int{"foo": 1, "bar": 2}` |
| add data |  `m["k2"] = 13` |
| find the length/number of values in the set | `len(m)` |
| delete a key/value pair | `delete(m, "k2")` |
| get the value of a key | `v1 := m["k2"]` |
| get value of a key & if the key exists | `v1, vExists := m["k2"]` |
| just check if the key exists | `_, vExists := m["k2"]` |

example: 
```Go
package main

import (
	"fmt"
	"strconv"
)

func main() {
	test := make(map[int]string)
	for i := 0; i < 10; i++ {
		test[i] = "something " + strconv.Itoa(i)
	}
	for i := range test {
		fmt.Println("line: ", test[i])
	}
	fmt.Println("test: ", test)
}
```