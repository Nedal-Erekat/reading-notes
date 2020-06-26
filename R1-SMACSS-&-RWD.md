# RWD
## Responsive Overview
#### Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.
## Responsive vs. Adaptive vs. Mobile
#### Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.
# Flexible Layouts
### Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.
1. Flexible Grid
#### Taking the flexible layout concept, and formula, and reapplying it to all parts of a grid will create a completely dynamic website, scaling to every viewport size. For even more control within a flexible layout, you can also leverage the min-width, max-width, min-height, and max-height properties.
> The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.
2. Media Queries
- Viewport Height & Width: `<meta name="viewport" content="width=device-width">`.
- Viewport Scale : `<meta name="viewport" content="initial-scale=2">`.
- Viewport Resolution : `<meta name="viewport" content="target-densitydpi=device-dpi">`.
- Combining Viewport Values : `<meta name="viewport" content="width=device-width, initial-scale=1">`.
3. Flexible Media
#### The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

#### One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.

> img, video, canvas {
  max-width: 100%;
}
