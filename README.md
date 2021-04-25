# This is an example site for Sass integration in Jekyll

## Overview

You have two kinds of Sass files:

1. Main files, which you wish to be output as CSS files
2. Partials, which are used by main files in `@import` statements

Main files are like pages – they go where you want them to be output, and they contain the YAML front matter (`---` lines) at the top.  
Partials are like hidden Jekyll data, so they go in an underscored directory, which defaults to `_sass`.  
In this project we changed the default setting, see [_config.yml](_config.yml) file.  
The site structure respect the 7-1 Pattern and look like this:  

    .
    | - assets/sass
      | - abstracts
        | - _variables.scss
      | - base
        | - _typography.scss
      | - layout
        | - _header.scss
        | - _footer.scss
      | - _main.scss
    | - assets/css
      | - styles.scss

And so on.

The output, in your `_site` directory, would look like this:

    .
    | - assets/css
      | - styles.css

That's it! Now you have just converted your SCSS/Sass 7-1 Pattern project over to CSS with all the proper inputs using Jekyll convention.

## Official documentation

<https://jekyllrb.com/docs/assets/>
