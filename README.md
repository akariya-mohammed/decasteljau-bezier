# De Casteljau / Bézier demo

Small demo I made for the Splines lecture to understand how Bézier curves
actually get built.

I kept getting confused by the Bernstein formula, so instead of just plotting
the final curve I wanted to *see* the De Casteljau steps. You drag the control
points and move the t slider, and the colored lines show the repeated linear
interpolation: each level just slides t along the segments until there's one
point left, which is the point on the curve.

The thing that finally made it click for me is that every step is just a lerp
between two points, so the curve can never leave the shape made by the control
points (the convex hull). I added the Bernstein weight bars and the basis plot
on the side to connect it back to the formula from the slides.

Just open `index.html` in a browser, no install needed.
