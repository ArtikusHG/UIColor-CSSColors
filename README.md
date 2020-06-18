# UIColor-CSSColors
Parses CSS strings into UIColor objects. "Inspired" by (and credit for the list of the W3C colors goes to) [UIColor+HTMLColors](https://github.com/jlawton/UIColor-HTMLColors).

# Usage
This library has one universal function:
```
[UIColor colorWithCSS:];
```
All you have to do, is use it with a CSS string, which can be HEX, RGB, HSL or a W3C color name:
```
// hex
[UIColor colorWithCSS:@"#272d3a"];
// rgb and rgba
[UIColor colorWithCSS:@"rgb(255, 50%, 80)"];
[UIColor colorWithCSS:@"rgba(255, 50%, 80, 0.8)"];
// hsl and hsla
[UIColor colorWithCSS:@"hsl(360, 30, 40)"];
[UIColor colorWithCSS:@"rgba(360, 30, 40, 0.8)"];
// W3C colors
[UIColor colorWithCSS:@"Black"];
[UIColor colorWithCSS:@"yellow"];
```

This library does not support all of the UIColor+HTMLColors features, like the NSScanner ones. However, the colorWithCSS: function should work the same way. I only wrote this because I needed a library with the same purpose as UIColor+HTMLColors, but the latter didn't compile with ARC and was simply outdated in general.
