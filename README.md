## 3D Spline Animation

##### LIVE DEMO: http://bullen.io/3d-spline-animation/demo.html

Hand-rolled demo for animating ordinary HTML elements with plain, no-library Javascript. It can make use of almost any CSS property that makes sense to animate, including fonts and the 3D properties. Each CSS  property animates across its own randomly-generated spline (anywhere from a cubic bézier to a 10th or 12th degree spline).

Animating a `<div>` (or similar element) this way lets you preserve links, photos, etc. inside the animated element, without needing to get into the intricacies of using a `<canvas>` element or keyframes, and without taking on the overhead of using one of the more complicated animation libraries.

This would probably be most useful for adding a few fast, lightweight animated elements to an otherwise static page. It has not been tested for heavier lifting like HTML game design or animated scientific graphing, but that might be the next place to take it.

In the [live demo](http://bullen.io/3d-spline-animation/demo.html) page, click the "ready!" button, which sets 50 `<div>` elements into simultaneous animation across several CSS properties (top, left, background color, border radius, and rotate X, Y, Z). The console log tracks the average animation time for each element. So far, in newer browsers, that has averaged around 16.5ms on my machines.
