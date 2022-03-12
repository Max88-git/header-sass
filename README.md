# Cloudcraft - Sass landing page

This is a Sass landing page solution. This was my first introduction to Sass, and I used it to design a landing page header that displayed variables, nesting, mixins, and functions, among other things.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learnt](#what-i-learnt)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [License](#license)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- Hover over the navbar and links

### Links

- GitHub URL: [Code](https://github.com/Max88-git/header-sass)
- Live Site URL: [Live Site](https://max88-git.github.io/header-sass/)

## My process

### Built with

- Semantic HTML5 markup
- Custom CSS properties
- Sass (Syntactically Awesome Style Sheets)

### What I learnt

- I learned how to use the $ symbol to construct variables.
- I learned how to nest selectors in the parent, making it a lot easier and avoiding having to repeat the same selector over and over again.
- I discovered how to make partials. They are little CSS snippets that can be used in other Sass files.
- Discussed mixins and functions, which allow you to design CSS blocks that may be run anywhere.
- Mixins allow you to create reusable styles that may be used across your CSS. The use of functions makes it simple to abstract out common formulas and actions in a legible manner.
- I learned about inheritance - You can construct the base styles for a button, for example, and then use @extend to extend the styling to other classes.

Here is a code snippet I am proud of:

```scss
// Margin & padding classes
$spaceamounts: (1, 2, 3, 4, 5);

@each $space in $spaceamounts {
  .m-#{$space} {
    margin: #{$space}rem;
  }
  .my-#{$space} {
    margin: #{$space}rem 0;
  }

  .p-#{$space} {
    padding: #{$space}rem;
  }
  .py-#{$space} {
    padding: #{$space}rem 0;
  }
}
```

### Useful resources

- [@extend rule](https://sass-lang.com/documentation/at-rules/extend) - The @extend rule in Sass instructs the language that one selection should inherit the styles of another.
- [@if and @else rules](https://sass-lang.com/documentation/at-rules/control/if#else) - We can utilise expressions in Sass. If the expression returns true, the block is evaluated; if the expression returns false, the block is not evaluated.
- [Partials](https://sass-lang.com/guide#topic-4) - A partial is a Sass file with an underscore in the name. You may call it \_partial.scss or something similar. The underscore informs Sass that the file is merely a portion of a larger file and should not be converted to CSS.

## Author

- Website - [Max Lockwood](https://www.maxlockwood.uk/)

## License

This project is licensed under the terms of the MIT license. A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code.

MIT &#169; Max Lockwood
