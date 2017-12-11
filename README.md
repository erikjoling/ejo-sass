# Ejo Sass Lib
A minimalistic Sass library for making CSS and SASS life easier. I see Sass as a way to write browserconsistent CSS. This library makes this process easier and more maintainable. 

Version: 2017-12-11  
Author: Erik Joling <erik@ejoweb.nl>

Note: Some of these packages prevent the redundancy of writing extensive code over and over again. But I think this should be handled by your editor via code-snippets. I think it's unnecessary to distantiate from vanilla CSS for this reason. 

Note: The two reasons I use sass are: 
    1) to centralize layout and styling settings.*
    2) to have extra control of writing browserconsistent CSS.**

*  I could also use helper classes or variables for this reason (NO! -->). The downside is that I need to add this to my HTML and I don't want that, because it fades the line between content and styling. 
** Flexbox in IE10/11 needs an additional max-width/height property for example. With Sass I can easily add this to the flex-item mixin. 

## Package
This library consists of multiple (largely) independant functionalities. 

### Borders - `_borders.scss`
Define borderstyles in your settings file. Use functions like @border or @border-width to write your borders.

### Breakpoints - `_breakpoints.scss`
Make it easier to use breakpoints. (Maybe remove, because I could also write this manually and add as a code-snippet)

### Colors - `_colors.scss`
Centralize the color palette, ie. multiple main colors and their variants

### Helpers - `helpers.scss`
Helper functions to make my Sass life easier

@functions: `strip-units`, `rem`, `em`, `shade`, `tint`  
@mixins: `on-event`  

### Icons - `_icons.scss`
Easy and consistent access to font-awesome icons

### Site Padding - `_site-padding.scss`
Centralize the padding to the horizontal sides of the websites. Has support for breakpoints (which is the reason it exists).

### Spaces - `_spaces.scss`
Use `v-space` and `h-space` to create consistent space-sizes over the entire website.

### Typography - `_typography.scss`
Create a consistent typography structure. Define you fonts (family, weights, styles) in your settings and use the mixins and functions in your Sass