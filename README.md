# Frontend Masters: CSS Grids and Flexbox in Responsive Web Design workshop files

Taught October 3-4, 2017, at Frontend Masters

Course is located here: https://frontendmasters.com/courses/css-grids-flexbox/

- [Code & Slides](https://github.com/jen4web/fem-layout/)

## Introduction

### Responsive Design

#### Flexible grid-based layout

![Grid-based layout](images/GridBasedLayout.png)

#### Media queries (CSS3)

- Browser reports screen resolution
- Based on current width, serve a stylesheet with layout for that width
- No Javascript involved

#### Images that resize

Images should change size, based on your screen resolution.

Solutions available client side and server side, including new `<picture>` tag

## Floats

Float is a hack, it where intended to do was float an image on a web page and wrap the text around it. It was not intended to layout whole web pages.

They have rows and cells

IF YOU FLOAT YOU MUST CLEAR

Source ordering determines display. Somoe rearrangement is possible.

Major disadvantage: equal column heights

![Float Layout Problem](images/FloatLayoutProblem.png)

### clear

> The clear CSS property sets whether an element must be moved below (cleared) floating elements that precede it. The clear property applies to floating and non-floating elements.

A common pattern is to clear the ::after pseudo-element of a row and add a block display
