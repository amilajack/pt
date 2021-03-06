# Release notes

## v0.2.0
**Mobile**
- Pt now supports multi-touch interactions and retina resolutions for mobile. Yay! Get started with this quick [mobile guide](http://williamngan.github.io/pt/docs/guide/mobile.html).

**Improvements**
- `Space` constructors get a complete makeover, making it simpler and clearer to use (Issue [#12](https://github.com/williamngan/pt/issues/12) and [#13](https://github.com/williamngan/pt/issues/13))
- New guides on [mobile](http://williamngan.github.io/pt/docs/guide/mobile.html) and [svg](http://williamngan.github.io/pt/docs/guide/svg.html)
- Updated documentations and fixed navigation issues in docs
- Improved SVG and DOM code. SVG moved to `core` library.
- New demos: [Delaunay triangles](http://williamngan.github.io/pt/demo/index.html?name=delaunay.generate) and [Game of Life](http://williamngan.github.io/pt/demo/index.html?name=grid.canFit)
- Various bug fixes

**Breaking changes**
- `CanvasSpace` and `SVGSpace` now uses a new constructor function. Please take a look at [migration guide](http://williamngan.github.io/pt/docs/guide/migration.html) and update your code.

## v0.1.1
**SVG!**
- Pt now supports both html5 canvas and svg. To render in svg, you can simply replace `CanvasSpace` and `Form` with `SVGSpace` and `SVGForm`, and just an additional line of `form.scope(...)` in your code. Everything else stays the same. See  demos [here](http://williamngan.github.io/pt/demo/index.html?name=svgform.scope) and [here](http://williamngan.github.io/pt/demo/index.html?name=svgform.circle).

**Extended documentations**
- [Documentations page]((http://williamngan.github.io/pt/docs/) now includes a section on extended Pt classes such as SVGForm and Noise.

**Bug fixes**
- improved gulp error handling
- improved homepage design
- other minor stuff


## v0.1 [experimental]
> The world was so recent that many things lacked names, and in order to indicate them it was necessary to point.  
> -- Gabriel Garcia Marquez

**What's new**
- The first release of Pt include a core set of classes based on Point, Form, and Space. 
- A couple of extended classes are in progress
- Draft of supporting documentations and demos

**What's missing**
- In this version we only provides `CanvasSpace` and `Form` to support html5 canvas drawing. 
We would want to get to other forms of expressions, such as DOM or SVG or even something more experimental like Sound.
- For canvas drawing, current release only supports 2D graphics for the most part. 
Needs some more thinking on the approach to 3D.
- Rough build system and unit tests. To be improved.
