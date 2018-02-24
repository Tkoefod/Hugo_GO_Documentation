---
title: "Regular Expressions"
lesson: 2
chapter: 5
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "tech"
type: "lesson"
tags:
    - programming
    - channels
    - filesystem
---

### Regular Expressions

* use the package: 'regexp'

[Go By Example on Regular Expressions](https://gobyexample.com/regular-expressions)

#### Tests if a pattern matches a string
```
match, _ := regexp.MatchString("p([a-z]+)ch", "peach")
```

#### Compile a regular expression for use in others

```
r, _ := regexp.Compile("p([a-z]+)ch")
```


 [online Go regex tester](https://regex-golang.appspot.com/assets/html/index.html)