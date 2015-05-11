> NOTE: If you're looking for [Facebook's IDE for React Native](http://nuclide.io/),
you're in the wrong place! Different project!

# nuclide

a CSS framework for utilizing the Atomic design pattern

### Summary

nuclide is a responsive, mobile-first, [Sass-based](http://sass-lang.com/) CSS framework
that follows Atomic design conventions.

It was designed out of the desire for a CSS framework that's **powerful**, **flexible**,
**maintainable**, **extensible**, and **easy to trace and comprehend**.

nuclide was developed while working on a slew of large, design-heavy websites and webapps,
and it's catered towards front-end developers and designers who need to implement designs
quickly while also producing clean, quality code. It works especially well on projects in
which designs are created beforehand and must then be implemented in HTML/CSS.

### Why should I use it?

- **It's powerful**: the Atomic design pattern, combined with programmatic generation of styles (colors and color variations, sizing units, fonts and font sizes, etc.) based on your configuration, removes much of the work of classical CSS frameworks
- **It's simple**: following Atomic conventions makes your HTML descriptive, your styles easily traceable, and cross-referencing specific properties across elements and components a breeze
- **It's smart**: nuclide leverages the concepts of composition and inheritance to create combinations of styles that draw from base Atomic classes, making Molecule creation powerful and intuitive

nuclide can give you the **freedom** and **flexibility** not provided by frameworks like
[Bootstrap](http://getbootstrap.com/) and [Foundation](http://foundation.zurb.com/).

### How do I use it?

nuclide uses modern Sass features, so make sure you have **Sass 3.3 or greater** installed.

- Download or clone nuclide
- `cd` into the `nuclide` directory and run `sass`, using the `--watch` option:

```
sass --watch lib/nuclide.scss:css/nuclide.css
```

- In the `lib` directory, tweak the `config`, `webfonts`, and other relevant Sass files with your own project's colors, values, fonts, and styles
- If you're using any Molecules, don't forget to `@import` them within `nuclide.scss`

nuclide will generate a slew of Atomic classes for you, many of them responsive (and
mobile-first) in nature, allowing you to design from the ground up across devices:

```html
<div class="m-sm-mobile m-lg-tablet m-xl-desktop ta-c">
    <span class="fz-sm-mobile fz-lg-tablet fz-xl-desktop c-cornflower fw-5">just a test!</span>
</div>
```

**Go forth and code!**

Oh, nuclide also works great with [trg](https://github.com/jkymarsh/tiny-responsive-grid) and
[lament configurator](https://github.com/jkymarsh/lament-configurator)!

### Molecules

Molecules are combinations of Atomic classes used in conjunction to form more complex
components, such as navigation, media elements, styled tables, buttons, form elements, and
so on.

One intent of nuclide is to create a basis of common Atomic classes from which other
developers and designers will create beautiful, elegant, responsive Molecules and share
them with the community!

Check out the [nuclide-molecules](https://github.com/jkymarsh/nuclide-molecules) repo for
sample Molecules.

### Caveats

- nuclide doesn't include a normalize, reset, grid, etc. Don't forget to include your favorites!
- Unfortunately, Sass doesn't currently support the use of `@extend` within media queries, which hampers nuclide's ability to be 100% inheritance-based, particularly for Molecules. [They're working on it](https://github.com/sass/sass/issues/1050).

### Inspiration and sources

- Class names and styles from the [Emmet toolkit](http://docs.emmet.io/cheat-sheet/)
- Structure and convention concepts from [inuit-css](https://github.com/csswizardry/inuit.css/)
- Basis for other styles from [nemophrost's atomic-css project](https://github.com/nemophrost/atomic-css)

### Atomic CSS resources

- http://bradfrostweb.com/blog/post/atomic-web-design/
- https://www.lucidchart.com/techblog/2014/01/31/atomic-css-tool-set/
- http://www.smashingmagazine.com/2013/10/21/challenging-css-best-practices-atomic-approach/
- http://www.smashingmagazine.com/2013/08/02/other-interface-atomic-design-sass/
- http://krasimir.github.io/organic-css/
- http://java.dzone.com/articles/atomic-css-tool-set
