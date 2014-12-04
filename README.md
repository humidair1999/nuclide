> NOTE: nuclide is a work in progress! Many features still forthcoming!

# nuclide

A CSS framework for utilizing the Atomic design pattern

### Summary

nuclide is a Sass-based CSS framework that attempts to follow Atomic CSS design
conventions.

Its emphasis is simplicity: it will not include fancy modals, form validation
elements, and so on; leave those things to frameworks and libraries like
Bootstrap and Foundation. nuclide offers a generalized set of classes to make
quickly building rock-solid layouts a breeze, without bogging you down too much
with the fancy widgets other libraries offer.

nuclide will eventually contain both atomic and molecular units:

- **atoms**, for providing individual styles with which you can compose elements
- **molecules**, for providing pre-determined combinations of atoms, representing commonly-used sets of styles

### How to use

The source for nuclide is implemented in [Sass](http://sass-lang.com/).

Assuming you have Sass installed via Rubygems, either compile the source Sass:

```
sass src/main.scss dest/nuclide.css
```

or use the `watch` directive from the command line:

```
sass --watch src/main.scss:dest/nuclide.css
```

Alternatively, you can grab the compiled `nuclide.css` in the `dest` directory and
replace any unit values manually.

Don't forget to add a [normalize](http://necolas.github.io/normalize.css/) and
[grid](http://responsive.gs/), also!

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
