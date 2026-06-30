# De Casteljau's Algorithm — Interactive Bézier Demo

An interactive demo built for the **Computer Graphics** course (Splines lecture).

It builds a Bézier curve the way it was taught in class: by **repeated linear
interpolation** (De Casteljau's algorithm). Drag the control points and move `t` —
the colored scaffold shows the nested interpolations collapsing to a single point on
the curve, so you can see *why* a Bézier curve is just nested lerps and why it always
stays inside the convex hull of its control points.

The side panel connects the geometric construction to the math: the Bernstein weights
`Bᵢⁿ(t)` (which sum to 1 — partition of unity) and the basis-function plot.

**Live demo:** open `index.html`, or visit the GitHub Pages link.

No dependencies — a single self-contained HTML file.
