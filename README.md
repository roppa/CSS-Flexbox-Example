This article was first written 4 years ago. Since then flex has become standard in things like react native. I had moved away from front end stuff only to come back to work on a react native app so had to start flexing again.

Let's be honest, CSS float layouts were a nightmare. Absolute and relative positioned things we won't say anything about. And ```display: table``` just feels really dirty. I mean **really** dirty. Especially when you started out using tables for layouts (I even felt dirty doing that, even though others felt it was fine).

There was always a designer who insists that content order is rearranged depending on the device - content in a different order on mobile vs desktop. That "dirty" feeling starts to surround me.

**NOW CAN WE PLEASE START USING FLEXBOX?** &hellip; or [grid](http://www.w3.org/TR/2015/WD-css-grid-1-20150917/) :-)

I say f*ck it. We are all about progressive enhancement and have been for years. I say if you want to work on bleeding edge projects then use it. If there is money riding on older browsers, then that's too bad, use the dirty table layout. But thankfully things like React native are using it!

Flexbox is a flexible **layout system** (an algorithm for positioning elements, whether floated, inline, table, grid) add on. So when I say **flexible** layout system, I mean flexible in lots of ways. Reordering content is a breeze. Resizing is a pleasure.

It is a little tricky to get your head around it to begin with, like a lot of things in the industry, so first I'd suggest going through some of the resources below to get a good grounding.

## Terminology

<dl>
  <dt>axis</dt>
  <dd>the flow in which elements flow, vertical or horizontal<dd>
  <dt>cross axis</dt>
  <dd>opposite to the parent axis<dd>
  <dt>flex-container</dt>
  <dd>a parent container that contains flexible child <b>flex-items</b></dd>
  <dt>flex-items</dt>
  <dd>nested child elements that adjust to parents size</dd>
</dl>

## Basics

Layouts are based on parent layout containers and flexible child containers. What this means is when the parent containers are resized, the children automatically adjust.

You start off with a container element, a **flex container**, and set the display attribute like so: ``` display: flex; ``` (add any browser prefixes as necessary). You can also set it to ```display: inline-flex``` if you want it to be inline. Then we can go ahead and fill it with child elements. You don't have to specify any attributes on the child elements, they will automatically become child flex items.

There is another concept to cover - the main and cross axis. X and Y if you like. This is the flow direction, either x or y, main or cross.

## Examples

- [Layout example](./examples/layout/index.html)

## Resources

- [Flexbox.io](http://flexbox.io/)
- [Scotch.io tutorial](https://scotch.io/tutorials/a-visual-guide-to-css3-flexbox-properties)
- [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Mozilla](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Flexible_boxes)
- [W3.org](http://www.w3.org/TR/css3-flexbox/)