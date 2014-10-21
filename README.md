> NOTE: nuclide is a work in progress! Many features still forthcoming!

# nuclide

A CSS framework for utilizing the Atomic design pattern

### How to use

The source for nuclide is implemented in [Sass](http://sass-lang.com/).

Assuming you have Sass installed via Rubygems, either compile the source Sass:

```
sass src/main.scss dest/style.css
```

or use the `watch` directive from the command line:

```
sass --watch src/main.scss:dest/style.css
```

Alternatively, you can grab the compiled `style.css` in the `dest` directory and
replace any unit values manually.

### What's included

- Basis for many styles and naming conventions from [nemophrost's atomic-css project](https://github.com/nemophrost/atomic-css)
- [normalize.css](https://github.com/necolas/normalize.css)
- [responsive grid system](http://responsive.gs/)
- Snippets from [HTML5 Boilerplate](http://html5boilerplate.com/)
