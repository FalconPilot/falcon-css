<div style="text-align: center">
  <img src="https://image.noelshack.com/fichiers/2018/01/3/1514992470-falconcss.png" alt="FalconCSS" style="width: 200px"/>
</div>

# Falcon CSS Library

I originally wrote this library for personal use. If you want to import it
yourself, feel free to do so :)

It's based on a strong usage of flexboxes to quickly and efficiently display
interface elements without requiring too much thinking or tinkering.

# General documentation

Here is a general documentation to be able to use efficiently the library.

## Flex container definitions

* `flex-row` [__class__]

Define a flex container with row-aligned children.

___Example___
```html
<div class="flex-row">(...)</div>
```
---
* `flex-col` [__class__]

Define a flex container with column-aligned children.

___Example___
```html
<div class="flex-col">(...)</div>
```

## Flex container children alignments

### Important note

Those classes are used to align flex container children whatever its flex
direction might be. It works as well with a container using `flex-row`,
`flex-col`, etc...

---
* `center-v` [__class__]

Vertically center the children of a flex container.

___Example___
```html
<div class="flex-row center-v">(...)</div>
```
---
* `center-h` [__class__]

Horizontally center the children of a flex container.

___Example___
```html
<div class="flex-row center-h">(...)</div>
```
---
* `flex-middle` [__class__]

This class is just an equivalent of `center-v center-h`. It's used mostly to
save space and avoid very long CSS classlists.

___Example___
```html
<div class="flex-col flex-middle">(...)</div>

<!-- Both of those lines render absolutely the same way -->

<div class="flex-col center-v center-h">(...)</div>
```
---
* `flex-top` [__class__]

Vertically align the children of a flex container from its top border.

___Example___
```html
<div class="flex-row flex-top">(...)</div>
```
---
* `flex-bottom` [__class__]

Vertically align the children of a flex container from its bottom border.

___Example___
```html
<div class="flex-row flex-bottom">(...)</div>
```
---
* `flex-left` [__class__]

Horizontally align the children of a flex container from its left border.

___Example___
```html
<div class="flex-row flex-left">(...)</div>
```
---
* `flex-right` [__class__]

Horizontally align the children of a flex container from its right border.

___Example___
```html
<div class="flex-col flex-right">(...)</div>
```
