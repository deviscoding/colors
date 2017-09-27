# StrapLess Colors
SASS color functions and maps used in StrapLess components.

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
Adds a provided map of `key: color` to the theme colors map.

`colors-merge($new-map)` -
Adds a provided map of `key: color` to the colors map.

`grays-merge($new-map)` -
Adds a provided map of `value: color` to the grays map.

`isLight($color-value)` - 
Determines if the given color value is a light color or a dark color.
