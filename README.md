# Animating HTML5 DOM Elements in 3D

CSS3 transitions/easing patterns have their limits. It's typically difficult to transition or animate an element with anything more complicated than a cubic spline, if you're not using a `<canvas>` element, or setting up an intricate series of keyframes. Using a `<canvas>` element, however, typically means that links, photos, HTML, etc. will not be easy, or even possible, to use inside it. More robust libraries such as OpenGL or WebGL carry too much overhead for a small site or one-page app. Meaning, if you want an element to swoop across the page along a complex curve, or transition multiple colors in a unique way, that's going to be a challenge with out-of-the-box JavaScript libraries.

Once you open the page, click the "ready!" button, which sets 50 `<div>` elements into simultaneous animation across several CSS properties (top, left, background color, border radius, and rotate X, Y, Z). The console log tracks the average animation time for each element. So far, in newer browsers, that has averaged around 16.5ms on my system.

#### Try it out: http://bullen.io/3d-spline-animation/demo.html
