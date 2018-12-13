---
layout: post
title: "Marlon Uriarte, flag"
date: 2018-12-13
---

![U.S Flag Image](/images/UsFlag.png)

```
include image
size = 100
width = size * 1.9
height = size * 1.0

stripe-height = height / 13
star-base-width = width * 7/13
star-base-height = stripe-height * 13
star-base = rectangle(star-base-width ,star-base-height,"solid" ,"blue" )
base = rectangle(width ,height ,"solid" ,"red" )
stripe = rectangle(width, stripe-height, "solid", "white" )

half-width = width * 1/2


o = place-image(stripe, half-width, stripe-height * 1.5, base)
tw = place-image(stripe, half-width, stripe-height * 3.5, o)
th = place-image(stripe, half-width, stripe-height * 5.5, tw)
fo = place-image(stripe, half-width, stripe-height * 7.5, th )
fi = place-image(stripe, half-width, stripe-height * 9.5, fo)
all-stripes = place-image(stripe, half-width, stripe-height * 11.5, fi)
place-image(star-base, 0, 0, all-stripes)
```

