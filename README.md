<p align="center">
  <img src="https://image.noelshack.com/fichiers/2018/01/3/1514992470-falconcss.png" alt="FalconCSS"/>
</p>

# Falcon CSS Library

I originally wrote this library for personal use. If you want to import it
yourself, feel free to do so :)

It's based on a strong usage of flexboxes to quickly and efficiently display
interface elements without requiring too much thinking or tinkering.

# General documentation

Here is a general documentation to be able to use efficiently the library.

# Browser compatibility

This library should be compatible with any web browser that supports the
following elements :

- Flexboxes
- `vw`/`vh` measurement units

# Table of contents

* [Main structure](#main-structure)
  * [falcon-body](#falcon-body)

* [Flex container definitions](#flex-container-definitions)
  * [flex-row](#flex-row)
  * [flex-col](#flex-col)

* [Flex container children alignments](#flex-children-alignments)
  * [center-v](#center-v)
  * [center-h](#center-h)
  * [flex-middle](#flex-middle)
  * [flex-top](#flex-top)
  * [flex-bottom](#flex-bottom)
  * [flex-left](#flex-left)
  * [flex-right](#flex-right)

<a name="main-structure"/>

## Main structure

<a name="falcon-body"/>

* `#falcon-body` [__id__]

This optional - although highly recommended - ID can only be used on a
`body` tag. It ensures your webpage's body always at least fills in the
entire client's viewport.

___Example___
```html
<body id="falcon-body">(...)</body>
```
---

<a name="flex-container-definitions"/>

## Flex container definitions

<a name="flex-row"/>

* `.flex-row` [__class__]

Define a flex container with row-aligned children.

___Example___
```html
<div class="flex-row">(...)</div>
```
---

<a name="flex-col"/>

* `.flex-col` [__class__]

Define a flex container with column-aligned children.

___Example___
```html
<div class="flex-col">(...)</div>
```

<a name="flex-children-alignments"/>

## Flex container children alignments

### Important note

Those classes are used to align flex container children whatever its flex
direction might be. It works as well with a container using `flex-row`,
`flex-col`, etc...

---

<a name="center-v"/>

* `.center-v` [__class__]

Vertically center the children of a flex container.

___Example___
```html
<div class="flex-row center-v">(...)</div>
```
---

<a name="center-h"/>

* `.center-h` [__class__]

Horizontally center the children of a flex container.

___Example___
```html
<div class="flex-row center-h">(...)</div>
```
---

<a name="flex-middle"/>

* `.flex-middle` [__class__]

This class is just an equivalent of `center-v center-h`. It's used mostly to
save space and avoid very long CSS classlists.

___Example___
```html
<div class="flex-col flex-middle">(...)</div>

<!-- Both of those lines render absolutely the same way -->

<div class="flex-col center-v center-h">(...)</div>
```
---

<a name="flex-top"/>

* `.flex-top` [__class__]

Vertically align the children of a flex container from its top border.

___Example___
```html
<div class="flex-row flex-top">(...)</div>
```
---

<a name="flex-bottom"/>

* `.flex-bottom` [__class__]

Vertically align the children of a flex container from its bottom border.

___Example___
```html
<div class="flex-row flex-bottom">(...)</div>
```
---

<a name="flex-left"/>

* `.flex-left` [__class__]

Horizontally align the children of a flex container from its left border.

___Example___
```html
<div class="flex-row flex-left">(...)</div>
```
---

<a name="flex-right"/>

* `.flex-right` [__class__]

Horizontally align the children of a flex container from its right border.

___Example___
```html
<div class="flex-col flex-right">(...)</div>
```
