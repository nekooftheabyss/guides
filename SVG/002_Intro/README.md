# 2. Intro
The following is an example of an SVG file. Don't worry, we will discuss each component separately.

```xml
<svg width="100" height="100" stroke="pink" stroke-width="4" fill="violet">
   <rect x="25" y="25" width="50" height="50"  />
</svg>
```

<svg width="100" height="100" stroke="pink" stroke-width="4" fill="violet">
   <rect x="25" y="25" width="50" height="50"  />
</svg>

## The `<svg>` Element
SVGs are defined using the `<svg>` tag. So,

```xml
<svg></svg>
```

Boom, you now have your own SVG that does nothing!

## Giving it a size
Let's keep the "scalable" part away for now. To define the size of an SVG, we use the `width` and `height` attributes.

```xml
<svg width="100" height="100"></svg>
```

Cool, now you have a 100 pixel-large SVG image that still does nothing!

## Adding content
Each element of an SVG can be added as a child of the SVG element.

```xml
<svg>
<!--children go here-->
</svg>
```

For now, let us add a rectangle.

```xml
<svg width="100" height="100">
   <rect width="50" height="50"  />
</svg>
```

We have now created a rectangle that has half the width and height of our SVG. You should be seeing a black box at the moment.

## Reposition the rectangle

We can use the `x` and `y` attributes to define its starting position.

```xml
<svg width="100" height="100">
   <rect x="25" y="25" width="50" height="50"  />
</svg>
```

Now we have a rectangle at the center of the SVG image.

## Giving it some colors

Let's give the rectangle a border to make it cooler.

```xml
<svg width="100" height="100" stroke="pink">
   <rect x="25" y="25" width="50" height="50"  />
</svg>
```

The `stroke` attribute defines the color of the element's border. For now, we are applying stroke to the entire SVG image. We will learn about detailed stuff later.

Now that the rectangle has a border, let's change the fill color.

```xml
<svg width="100" height="100" stroke="pink" fill="violet">
   <rect x="25" y="25" width="50" height="50"  />
</svg>
```

Now we have a colorful rectangle in front of us.