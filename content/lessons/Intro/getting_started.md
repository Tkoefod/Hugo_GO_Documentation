---
title: "Getting Started"
lesson: 1
chapter: 1
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "tech"
type: "lesson"
tags:
    - programming
    - stuff
    - gettingStarted
---

In GO programmers use camel case for names so things like 'CamelCase' or 'camelCase' but not 'camel_case'.

#### Main types of Declarations:

| name | type | syntax | example |
| --- | --- | --- | --- |
| var | variable | var name type = expression | var myVar int = 5 |
| const | constant | const name type = expression | const myVar string = "something" |
| type | |
| func | function | func name (input_type) output_type { }|


#### Types of Variables

| name | type | example |
| --- | --- | --- |
| int | integer number | 25 |
| float64 | long 64 bit decimal | 1.01234 |
| string | string | "some string" |
| bool | boolean | true |


#### Ways to declare

```
var i, j, k int
const myConstant string = "some constant"
```
```
var b, f, g = true, 2.3, "text"
```

##### short variable declaration

these are very common although they can only be used inside a function and not globals.
```
variableName := "expression"
```

#### Multiple Declarations from a function

functions in GO can return more then one value thus declarations are flexible for that too.

```
f, g := os.Open(name)
```
so in the above example f & g are both declared and assigned in one line simply.
sadf


#### Included help files

you can use the `godoc <pkg>` command to get help on that package


