# goshawk

![goshawk](./img/goshawk.jpg)

wireless keyboard with distintive features rarely seen elsewhere

* split design, but only requires 1 controller/battery
* 8 physical rows mapped to 4 logical rows makes it easier to wire

splay and key layout inspired by [osprette](https://github.com/smores56/osprette) / [clog](https://github.com/smores56/clog-v2) and [lil chonky bois](https://github.com/sanderboer/chonkybois)

split inspired by [schrodinger](https://www.reddit.com/r/MechanicalKeyboards/comments/yrse5t/the_schrodinger_a_keyboard_thats_both_wired_and/)

## bom

| Syntax          | Quantity    | Link                                              |
| -----------     | ----------- | ----                                              |
| nice-nano       | 1           | https://nicekeyboards.com/nice-nano/#find-a-store |
| battery         | 1           | 601230                                            |
| idc cable board | 2           | https://www.adafruit.com/product/2743             |
| idc cable       | 1           | https://www.adafruit.com/product/5804             |
| power switch    | 1           | https://www.amazon.com/dp/B09R3ZWBBC              |

## build

see [build.md](./build.md)


## pinout

8 physical rows mapped to 4 logical rows. Rows 1-4 are left side, rows 5-8 are right side.

![pinout](./img/pinout.png)

## zmk config

https://github.com/taylorzr/zmk-config/tree/master/config/boards/shields/goshawk


## 3d model

https://cad.onshape.com/documents/b1a3d5d385ce946f6e9b2f83/w/2e8ce54f087bb732d581ef47/e/49486961fd79efcfe6401002?renderMode=0&uiState=65fc31cfc471200c6baa1e48


## v1 -> v2

problems with v1
- pins are fragile
- fitting pins into bottom is finicky
  - i printed at same size, and then lightly drilled out the holes, but it was difficult to get
    consistent tension
- spacing between columns felt slightly too large
- pinky column drop was slightly too small

v2 changes
- added perimeter wall and slight chamfer
- m3 screws instead of pins
  - M3 x D5 x L4.0 (same as lil chonky bois)
  - https://www.amazon.com/uxcell-Knurled-Insert-Female-Embedding/dp/B09MCW7ZN5/ref=sr_1_11?crid=2H9C0WO3CKSGJ&dib=eyJ2IjoiMSJ9.OJgPUS62VGOz_WdCphJqCPGR0mVngCvqhtk3wP61vT6sogorchuzJvzn0JLgjiF1guPqf5dstjvj6Ml3LqUNYP-11GjrMkGx3ArojjGzrKKhUvaRprb9CrVpEOXkSsgXfbbIMLlTrDiTdwVB9ywNIFcQzVIJ4QGc2EPums7LD5U8vyn1CSbVyWLDVtCgZH8I9-_IRrXfqueuqW8GCf6sYi84n8f9pLQKq5kBu6k-aDg.a4mjQzjd7THxeEgFk4dlfqCYnbyW-JPV-kRei-XcTgM&dib_tag=se&keywords=m3+x+d5+x+l4.0+knurled+inserts&qid=1711027812&sprefix=m3+x+d5+x+l4.0+knurled+insterst%2Caps%2C87&sr=8-11
- adjusting column and pinky spacing
- no interior supports
  - with the perimeter wall, I don't feel like the top plate is too weak
