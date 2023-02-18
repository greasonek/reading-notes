# Class 5 Reading Notes

## HTML Media

- <img> elements requires src and alt attributes

  - **src** contains URL pointing to the image - without this, img has no image to load

  - **alt** alternative text for the image in case it cannot be loaded or if a screen reader is needed. 

- use width and height attributes to specify size of image (Cmd + I) - if browser is slow with loading the image user will see a black space of the image size [*use CSS to alter image size*]

**< figure> and < figcaption> elements** - wrap entire img link in < figure> element and use the < figcaption> element to write a caption for the image

- A figure can be more than an image. Can also be audio, video, equation, table, etc. 

- **background-image!** -if used in CSS will not show up for screen readers. If image is meaningful to your content it should be used as an HTML image, if purely decoration it should be used in CSS

* **HOTLINKING** = pointing src attribute to an image hosted on someone else's website without permission (unethical!)

I###IMAGE TYPES

- must be downloaded before use

- BMP - uncompressed raster images

- GIF - supported by HTML; used for it's animation in social media for short videos, memes etc. ; good for simple images and animation

- ICO - designed by Microsoft for desktop icons of Windows. ICO file can contain BMP or PNG image

- JPEG - useful for photos

- PNG - 

- SVG - ideal for diagrams, icons, images that need to be accurately drawn at any size. 

- TIFF - stores scanned photos; larger than images in other formats. 

1. Alt attribute can be used if an image cannot load on a webpage due to poor internet connection. It is also useful for visually impaired users using a screen reader. 

2. Accessibility of an image in HTML can be achieved by using both the alt attribute and writing a caption for the image with a figcaption element. Alt text has the same functionality as an image when it's absent while a caption is beneficial to people who are visually impaired and those who are not. The alt text and the figcaption should not say the same thing. 

3. Figure element is useful in an HTML doc to link the figure to a caption. It provides a semantic container for the figure and is useful for screen readers to associate the caption with the image. 

4. GIF is best used for animation or creating short videos. It is very popular in current social media for its animation. SVG is best used for diagrams and icons, has no animation and works well for images that need to be drawn to any size. 

5. For screenshots, a lossless format is preferred. PNG is the best option or WebP so as to preserve the quality of the photo.

## CSS

1. Forground colors in an HTML doc are the text colors, background colors are the color of the area behind the text. 

2. To give a colorless blog some color, use the background-color styling to add background color, the color styling to add color to the text. Pick a base color to define the websit or subject matter. Utilize color theory from here to build a pallette of appropriate colors for the site. Add in neutral colors like black, white or gray but keep the total number of colors to a minimum to keep the site clean and easy to digest. Keep accessibility and color blindness in mind. **Never** use color as the only way to know something. 

3. The browser will only apply the text of your choosing if it's available on the machine the website is being accessed on, otherwise the browser will use a default font. Keep web safe fonts in mind. 

4. Font-size changes the size of the font, usually measured in px or em. Font-style is used to italicize. Font-weight sets the boldness of the text, this can be light, normal, bold, extrabold or black.

5. To add spacing around the characters of the h1 element by using letter-spacing and word-spacing properties. 



## Things I want to know more about 