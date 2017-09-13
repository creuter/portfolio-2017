---

title: Tint your gray text
date: 2017-08-28 14:01 UTC
tags: color, sass

---

Adding some color to your grays can add richness to visual design and make it
more lifelike. For text, we can keep that color cohesive with the rest of the
palette in a couple of ways.

Using [alpha transparency][rgba] will let a hint of whatever color is behind the
text show through:

```scss
$dark-gray: #333;
$base-font-color: rgba($dark-gray, 0.9);
```

Or, [mixing][mix] the gray with another prominent color will help maintain a
consistent hue:

```scss
$dark-gray: #333;
$body-background-color: #f7d1be;
$base-font-color: mix($body-background-color, $dark-gray, 10%);
```

[rgba]: https://developer.mozilla.org/en-US/docs/Web/CSS/color#rgba()
[mix]: http://sass-lang.com/documentation/Sass/Script/Functions.html#mix-instance_method
