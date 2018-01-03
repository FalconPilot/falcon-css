<p align="center">
  <img src="https://image.noelshack.com/fichiers/2018/01/3/1514992470-falconcss.png" alt="FalconCSS"/>
</p>

# Falcon CSS Library

I originally wrote this library for personal use. If you want to import it
yourself, feel free to do so :)

It's based on a strong usage of flexboxes to quickly and efficiently display
interface elements without requiring too much thinking or tinkering.

You can clone the repository and check the `demo.html` file to get an idea of
what an example page built only with very few complementary CSS looks like.

You can also look at the `demo.html` source code to get some inspiration if
you want.

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
  * [falcon-header](#falcon-header)
  * [falcon-container](#falcon-container)
  * [falcon-footer](#falcon-footer)

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

* [Title formatting classes](#title-formatting-classes)
  * [centered-title](#centered-title)

<a name="main-structure"/>

## Main structure

<a name="falcon-body"/>

* `#falcon-body` [__id__]

This optional - although highly recommended - ID can only be used on a
`body` tag. It ensures your webpage's body always at least fills in the
entire client's viewport.

When using this ID, it is advisable to use the following basic structuration
pattern on your webpage :

```html
<body id="falcon-body">
  <header id="falcon-header">(...)</header>
  <main id="falcon-container">(...)</main>
  <footer id="falcon-footer">(...)</footer>
</body>
```

___Usage example___
```html
<body id="falcon-body">(...)</body>
```
---

<a name="falcon-header"/>

* `#falcon-header` [__id__]

Only compatible with a `<header>` tag. Best used inside `#falcon-body`.

___Usage example___
```html
<header id="falcon-header">(...)</header>
```
---

<a name="falcon-container"/>

* `#falcon-container` [__id__]

Only compatible with a `<main>` tag. Best used inside `#falcon-body`.

___Usage example___
```html
<main id="falcon-container">(...)</main>
```
---

<a name="falcon-footer"/>

* `#falcon-footer` [__id__]

Only compatible with a `<footer>` tag. Best used inside `#falcon-body`.

___Usage example___
```html
<footer id="falcon-footer">(...)</footer>
```

<a name="flex-container-definitions"/>

## Flex container definitions

<a name="flex-row"/>

* `.flex-row` [__class__]

Define a flex container with row-aligned children.

___Usage example___
```html
<div class="flex-row">(...)</div>
```
---

<a name="flex-col"/>

* `.flex-col` [__class__]

Define a flex container with column-aligned children.

___Usage example___
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

___Usage example___
```html
<div class="flex-row center-v">(...)</div>
```
---

<a name="center-h"/>

* `.center-h` [__class__]

Horizontally center the children of a flex container.

___Usage example___
```html
<div class="flex-row center-h">(...)</div>
```
---

<a name="flex-middle"/>

* `.flex-middle` [__class__]

This class is just an equivalent of `center-v center-h`. It's used mostly to
save space and avoid very long CSS classlists.

___Usage example___
```html
<div class="flex-col flex-middle">(...)</div>

<!-- Both of those lines render absolutely the same way -->

<div class="flex-col center-v center-h">(...)</div>
```
---

<a name="flex-top"/>

* `.flex-top` [__class__]

Vertically align the children of a flex container from its top border.

___Usage example___
```html
<div class="flex-row flex-top">(...)</div>
```
---

<a name="flex-bottom"/>

* `.flex-bottom` [__class__]

Vertically align the children of a flex container from its bottom border.

___Usage example___
```html
<div class="flex-row flex-bottom">(...)</div>
```
---

<a name="flex-left"/>

* `.flex-left` [__class__]

Horizontally align the children of a flex container from its left border.

___Usage example___
```html
<div class="flex-row flex-left">(...)</div>
```
---

<a name="flex-right"/>

* `.flex-right` [__class__]

Horizontally align the children of a flex container from its right border.

___Usage example___
```html
<div class="flex-col flex-right">(...)</div>
```

<a name="title-formatting-classes"/>

## Title formatting classes

<a name="centered-title"/>

* `.centered-title` [__class__]

Define a title element as taking 100% of its parent width at least and
centering any of its inline children. This class is only compatible with the
`h1` to `h6` tags, for semantic purposes.

___Usage example___
```html
<h1 class="centered-title">(...)</h1>
```
