## 3D Spline Animation

##### LIVE DEMO: http://bullen.io/3d-spline-animation/demo.html

CODING ISSUE: CSS3 transitions/easing patterns have their limits. It's typically difficult to transition or animate an element with anything more complicated than a cubic spline, if you're not using a `<canvas>` element or setting up an intricate series of keyframes. Using a `<canvas>` element, however, typically means that links, photos, HTML, etc. will not be easy, or even possible, to use inside the `<canvas>` element. More robust libraries such as OpenGL or WebGL carry too much overhead for a small site or one-page app. So, if you want an element to swoop across the page along a complex curve, or transition multiple colors in a unique way, that's going to be a challenge with out-of-the-box coding.

HOW IT WORKS: The demo parses each element's computed style, organizes each CSS3 property to animate or transition into arrays and a master queue, then loops repeatedly through the final animation queue, inlining styles on JS-generated `<div>` elements. It can record the average animation time and the easing deltas, and save a snapshot of each element's animation details to a server in JSON format.

RESOURCES USED: Plain JavaScript. For the matrix math, I used a few portions of [gl-matrix](https://github.com/toji/gl-matrix), mostly because there aren't too many unique ways to do matrix math in JavaScript, and the functions in this library run very quickly and reliably. In terms of the CSS3 parsing and animation engine, it's my own work.

THE DEMO: In the [live demo](http://bullen.io/3d-spline-animation/demo.html) page, click the "ready!" button, which sets 50 `<div>` elements into simultaneous animation across several CSS properties (top, left, background color, border radius, and rotate X, Y, Z). The console log tracks the average animation time for each element. So far, in newer browsers, that has averaged around 16.5ms on my machines.
