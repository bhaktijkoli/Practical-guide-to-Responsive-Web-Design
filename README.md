# Practical Guide to Responsive Web Design

## Overview

## Table of Contents
- Viewport
- Media queries
- Breakpoints
- Mobile First
- Fluid Layouts
- Relative sizing

## View Port
A Browser’s viewport is the area of web page in which the content is visible to the user. The viewport does not have the same size, it varies with the variation in screen size of the devices on which the website is visible. For a laptop, the viewport has a larger size as compared to a smartphone or tablet.

<img src="https://i.stack.imgur.com/qP6La.png">

We can change / set the viewport using meta tag. Most commonly used settigns for viewport is as follows

```html
<meta name="viewport" content= "width=device-width, initial-scale=1.0">
```

Following settings are available:-
- **width**: Width of the virtual viewport of the device.
- **height**: Height of the virtual viewport of the device.
- **initial-scale**: Zoom level when the page is first visited.
- **minimum-scale**: Minimum zoom level to which a user can zoom the page.
- **maximum-scale**: Maximum zoom level to which a user can zoom the page.
- **user-scalable**: Flag which allows the device to zoom in or out.(value= yes/no).

## Media Queries
CSS Media queries are a way to target browser by certain characteristics, features, and user preferences, then apply styles or run other code based on those things.
Most commonly used to target viewport ranges
```css
/* When the browser is at least 600px and above */
@media screen and (min-width: 600px) {
  body {
    /* Apply some styles */
  }
}
```

### Components of Media Query
<img src="https://i0.wp.com/css-tricks.com/wp-content/uploads/2020/09/media-query-anatomy.jpg?resize=1000%2C66&ssl=1">

For Complete guide refer this [article](https://css-tricks.com/a-complete-guide-to-css-media-queries/)


## Breakpoints
CSS breakpoints are points where the website content responds according to the device width, allowing you to show the best possible layout to the user.
</br>
CSS breakpoints are also called media query breakpoints, as they are used with media query.

| Breakpoint  | Breaks At |
|-------------|-----------|
| Small       | 640       |
| Medium      | 768       |
| Large       | 1024      |
| Extra Large | 1280      |

## Mobile First
Mobile First Approach refers to the practice of designing and/or developing an online experience for mobile before designing for desktop web or any other device.

<img src="https://i0.wp.com/css-tricks.com/wp-content/uploads/2021/02/pasted-image-0.png?resize=549%2C240&ssl=1">

This means plan first for:-
- Small Screens
- Fat fingers
- Slow Connection
- A user in a hurry

By introducing constraints such as:-
- 3-Click Rule
- One-Thumb Rule
- Seconds rather than minutes  


## Fluid Layouts

A fluid layout is a type of webpage design in which layout of the page resizes as the window size is changed. This is accomplished by defining areas of the page using percentages instead of fixed pixel widths.

<img src="https://blog.hubspot.com/hs-fs/hubfs/Google%20Drive%20Integration/What%20Is%20Fluid%20Design,%20and%20How%20Is%20It%20Used%20on%20Websites%3F.png?width=1000&name=What%20Is%20Fluid%20Design,%20and%20How%20Is%20It%20Used%20on%20Websites%3F.png">

## Relative Sizing

Relative length units specify a length relative to another length property. Relative length units scale better between different rendering medium.

- **em** Relative to the font-size of the element (2em means 2 times the size of the current font)
- **ex** Relative to the x-height of the current font (rarely used)
- **cn** Relative to the width of the "o" (zero)
- **rem** Relative to font-size of the root element
- **vw** Relative to 1% of the width of the viewport*
- **vh** Relative to 1% of the height of the viewport*
- **vmin** Relative to 1% of viewport's* smaller dimension
- **vmax** Relative to 1% of viewport's* larger dimension
- **%** Relative to the parent element

For complete guide refer this [article](https://www.w3schools.com/cssref/css_units.asp)