## Animating DOM Elements in 3D

Regular CSS3 transitions/easing patterns are limited in scope, meaning, if you want an element to swoop across the page along a complex curve, or transition multiple colors in a unique way, that's going to be a challenge without some extra coding. This page was an experiment in creating complex animation paths in the browser using nothing more than ordinary `<div>` elements and pure JavaScript.

Once you open the page, click the "ready!" button, which sets 50 `<div>` elements into simultaneous animation across several CSS properties (top, left, background color, border radius, and rotate X, Y, Z). The console log tracks the average animation time for each element. So far, in newer browsers, that has averaged around 16.5ms on my system.

##### Try it out: www.matthewbullen.net/3d-spline-animation/demo.html
