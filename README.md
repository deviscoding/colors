# StrapLess Colors
SASS color functions and maps used in StrapLess components.  Can also be used quite effectively in any SASS where one desires an easy way to manage colors.

### Available Color Maps

Inclusion of the 'color-variables' establishes three color maps: `$grays`, `$colors`, and `$theme-colors`.

These color maps can be utilized and manipulated with various included functions.

### Available Functions

`color($name)` - 
Retrieves a color from the `$color` map by color name.

`theme-color($name)` -
Retrieves a color from the `$theme-colors` map by context name.

`gray($value)` -
Retrieves a shade from the `$grays` map by progression value, 50 - 900.

`set-color($name,$color-value)` -
Adds or sets a color by the name of `$name` to the colors map with the value `$color-value`. Any existing color with the same name will be overwritten.

`set-theme-color($name,$color-value)` -
Adds or sets a color by the name of `$name` to the theme colors map with the value `$color-value`. Any existing color with the same name will be overwritten.

`set-gray($value,$color-value)` -
Adds or sets a color by the name of `$value` to the gray shades map with the value `$color-value`. Any existing color with the same name will be overwritten.

`theme-colors-merge($new-map)` -
Adds a provided map of `key: color` to the theme colors map.  Any new theme-colors will be added to the existing map.  Any key that already exists will be overwritten with your new value.

`colors-merge($new-map)` -
Adds a provided map of `key: color` to the colors map. Any new colors will be added to the existing map.  Any key that already exists will be overwritten with your new value.

`grays-merge($new-map)` -
Adds a provided map of `value: color` to the grays map. Any gray values will be added to the existing map.  Any key that already exists will be overwritten with your new value.

`isLight($color-value)` - 
Determines if the given color value is a light color or a dark color.  Useful for setting foreground colors that contrast with background colors.

### How to Use

To use effectively, you should `@import "colors";` BEFORE any variables that set or utilize colors.  This will set the base colors and allow you to do the following:

* Use colors with the `color`, `theme-color`, and `gray` functions.
* Add or replace colors to the color map without worrying about `!default` by using the `set-*` functions.
* Merge maps of new colors with the existing maps without wiping anything out.


