> NOTE: If you're looking for [Facebook's IDE for React Native](http://nuclide.io/),
you're in the wrong place! Different project!

> NOTE: nuclide is a work in progress! It's not yet considered a stable release,
and should be treated as a **beta project**!

# nuclide

A CSS framework for utilizing the Atomic design pattern

### Summary

nuclide is a Sass-based CSS framework that follows Atomic CSS design conventions.

It has a few emphases:

- **simplicity:** all Atomic classes/rules should be easily traceable and clearly named
- **power:** Sass should be leveraged to programmatically generate classes, color variations, size variations, and more for us
- **inheritance/composition:** *molecules*, or elements composed of multiple *atoms*, should inherit from, and be composed by, multiple individual Atomic classes

nuclide was designed while working on various *custom*, *large-scale*, *intensive*
web applications. It's the perfect solution if you're looking for a powerful framework
that will give your CSS (and HTML!) **structure** and **convention** without cramping your style or forcing
you to adhere to (or heavily modify) pre-defined components or widgets.

### How to use

The source for nuclide is implemented in [Sass](http://sass-lang.com/).

Assuming you have Sass installed, either simply compile the source Sass:

```
sass lib/nuclide.scss css/nuclide.css
```

or use the `watch` directive from the command line:

```
sass --watch lib/nuclide.scss:css/nuclide.css
```

### Don't forget to add

- a grid of some sort (may I suggest [trg](https://github.com/jkymarsh/tiny-responsive-grid)?)
- a utility library for transformative UIs (may I suggest [lament configurator](https://github.com/jkymarsh/lament-configurator)?)
- a [normalize](http://necolas.github.io/normalize.css/) or [reset](http://meyerweb.com/eric/tools/css/reset/)

### Inspiration and sources

- Class names and styles from the [Emmet toolkit](http://docs.emmet.io/cheat-sheet/)
- Basis for other styles from [nemophrost's atomic-css project](https://github.com/nemophrost/atomic-css)

### Atomic CSS resources

- http://bradfrostweb.com/blog/post/atomic-web-design/
- https://www.lucidchart.com/techblog/2014/01/31/atomic-css-tool-set/
- http://www.smashingmagazine.com/2013/10/21/challenging-css-best-practices-atomic-approach/
- http://www.smashingmagazine.com/2013/08/02/other-interface-atomic-design-sass/
- http://krasimir.github.io/organic-css/
- http://java.dzone.com/articles/atomic-css-tool-set

### TODO: Upcoming

- Molecules via patterns from: http://pea.rs/
- Plugins for patterns implemented via: https://ux.mailchimp.com/patterns

### TODO: Philosophy

- All styles should be easily traceable - every root class in the Style panel should be an atomic one (e.g. `.button` traces down to `.d-b`, `.p-lg`, etc.)
- All styles that appear in the Style panel class lists should be usable; there shouldn't be any molecules
that are "incomplete" (e.g. an incomplete `.button` class that a complete class `.button--lg` extends)
- Every molecule should be 100% composed of individual atomic classes
- Every molecule should be top-level and usable regardless of HTML structure - NO NESTING/DESCENDANTS (exceptions: HTML elements with required structure (`ol`, `ul`, `dl`, etc.))
- Molecules should provide baseline, pragmatic, "80/20" functionality - no flair or edge cases
- Molecules should adhere to BEM methodology
