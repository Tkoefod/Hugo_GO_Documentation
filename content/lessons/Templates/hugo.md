---
title: "HUGO"
lesson: 4
chapter: 2
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "01/01/2017"
category: "tech"
type: "lesson"
tags:
    - programming
    - HUGO
    - templates
    - static
---

### HUGO is an exreamly fast wonderful static website generator

- (HUGO)[https://gohugo.io]

HUGO takes markdown files along with TOML, JSON, or YAML and feeds that through the templates to create the site.

## Types of Front Matter data types

Front Matter in HUGO is the data that is included at the top of the markdown file along with some predefined variables that HUGO provides.

### YAML (most common)
example: 
```
---
someKey: "value"
someNum: 45
someBool: true
---
```
[offical spec](http://yaml.org/spec/1.2/spec.html)
### TOML (very simular to YAML and older format)
example: 
```
+++
someKey = "value"
someNum = 45
someBool = true
+++
```
[offical spec](https://github.com/toml-lang/toml)
### JSON ( standard JSON )
example:
```
{
    someKey: "value",
    someNum: 45,
    someBool: true
}
```
[offical spec](https://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf)

