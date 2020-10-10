# Mustache.js
#### Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
#### It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
#### mustache.js is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating. And, since mustache supports various languages, we don’t need a separate templating system on the server side.
> `Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });// returns: Hello, Sherlynn`
# Flexbox
* Note that CSS columns have no effect on a flex container.
- display
#### This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

>.container { display: flex;  /* or inline-flex */ }
![flex](https://css-tricks.com/wp-content/uploads/2018/10/order.svg)
- order
#### By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.
> .item {order: 5; /* default is 0 */}
- flex-direction
#### This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.

> .container {flex-direction: row | row-reverse | column | column-reverse;}

- flex-grow

#### This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.

#### If all items have flex-grow set to 1, the remaining space in the container will be distributed equally to all children. If one of the children has a value of 2, the remaining space would take up twice as much space as the others (or it will try to, at least).

- flex-wrap
> .container { flex-wrap: nowrap | wrap | wrap-reverse; }
* nowrap (default): all flex items will be on one line
* wrap: flex items will wrap onto multiple lines, from top to bottom.
* wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

![q](https://css-tricks.com/wp-content/uploads/2018/10/flex-wrap.svg)

- justify-content
![q](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)
#### This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.
```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
 }
 ```
* flex-start (default): items are packed toward the start of the flex-direction.
* flex-end: items are packed toward the end of the flex-direction.
* start: items are packed toward the start of the writing-mode direction.
* end: items are packed toward the end of the writing-mode direction.
* left: items are packed toward left edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.
* right: items are packed toward right edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.
* center: items are centered along the line
space-between: items are evenly distributed in the line; first item is on the start line, last item on the end line
* space-around: items are evenly distributed in the line with equal space around them. Note that visually the spaces aren’t equal, since all the items have equal space on both sides. The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.
* space-evenly: items are distributed so that the spacing between any two items (and the space to the edges) is equal.
![qq](https://css-tricks.com/wp-content/uploads/2018/10/align-content.svg)