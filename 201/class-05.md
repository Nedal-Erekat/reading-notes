# Images
#### If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.

### Add image:
#### To add an image into the page you need to use an `<img>` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:
1.  `src` This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.
2. `alt` This provides a text description of the image which describes the image if you cannot see it.
3. `title` You can also use the title attribute with the `<img>` element to provide additional information about the image.
4. `height` This specifies the height of the image in pixels.
5. `width` This specifies the width of the image in pixels.
> `<img src="images/quokka.jpg" alt="A family of quokka" width="600" height="450" />`
6. `align`   chapter-05/aligning-images-horizontally.html HTML The align attribute was  commonly used to indicate how  the other parts of a page should  flow around an image.

### HTML5: Figure and Figure Caption
#### Images often come with captions. HTML5 has introduced a new `<figure> `element to contain images and their caption so that the two are associated. `<figcaption>`
> <figure>
> <img src="images/otters.jpg" alt="Photograph of
>  two sea otters floating in water">
> <br />
>  <figcaption>Sea otters hold hands when they
>  sleep so they don't drift away from each
>  other.</figcaption>
> </figure>

### CSS3: Opacity opacity, rgba
#### CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

### CSS3: HSL & HSLA hsl, hsla:
1. hue :This is expressed as an angle (between 0 and 360 degrees).
2. saturation :This is expressed as apercentage.
3. lightnessL This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black. 4 
4. alpha This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0 75 represents 75% transparency

### Fonts
#### There are properties to control the choice of font, size,
weight, style, and spacing.
1.  There is a limited choice of fonts that you can assume most people will have installed.
2. If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
3. You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
4. You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, orwhen they have visited a link.