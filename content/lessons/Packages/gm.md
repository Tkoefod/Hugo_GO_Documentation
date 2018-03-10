---
title: "Graphic Magic"
lesson: 1
chapter: 10
cover: "https://unsplash.it/400/300/?random?BoldMage"
date: "03/01/2018"
category: "golang"
type: "lesson"
tags:
     - programming
     - images
---

## GraphicsMagic

- [gm main site](http://aheckmann.github.io/gm/)
- [gm golang bindings site](https://github.com/gographics/gmagick)

example: 
```Go
package main

import (
    "flag"
    "github.com/gographics/gmagick"
)

func resize(orig string, dest string) {
    mw := gmagick.NewMagickWand()
    defer mw.Destroy()
    mw.ReadImage(orig)
    filter := gmagick.FILTER_LANCZOS
    w := mw.GetImageWidth()
    h := mw.GetImageHeight()
    mw.ResizeImage(w/2, h/2, filter, 1)
    mw.WriteImage(dest)
}

func main() {
    f := flag.String("from", "", "original image file ...")
    t := flag.String("to", "", "target file ...")
    flag.Parse()

    gmagick.Initialize()
    defer gmagick.Terminate()

    resize(*f, *t)
}
```

so the command to use would be: `thisProgram -from <somefile.jpg> -to <newfile.jpg>`