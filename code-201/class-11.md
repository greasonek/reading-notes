# Class 11 Reading Notes

## Video and Audio Content

- <video> allows to embed video with src and controls

- container formats - include MP3, MP4 and WebM - define structure the video/audio traacks are stored along with metadata describing the media, etc. 

1. Video and audio in the early 2000s had security and accessibility issues and have been replaced by <video> and <audio> elements and the JavaScript API's that control them.

2. src attribute creates a path to the video being embeded. Controls allow the user to control the video and audio so they can start, stop, and adjust the volume of the video. This is especially important for people with epilepsy. Controls attribute includes a control interface, or the interface can be built using a JavaScript API.

3. Fallback content inside the <video> element will be displayed if the page doesn't support the video element. This can be a direct link to the video file.

4. Video is Batmnan and audio is Robin.

## Guide to Grid

- Define container element with **display: grid**; set columns and row sizes with **grid-template-columns** and **grid-template-rows** - child elements = *grid-column and grid-row*

1. Grid is a two-dimensional system that spaces items in rows and columns while Flexbox is one-dimensional and works with elements in linear order.

2. Grid container - defines the element container with display:grid. This is the parent of all grid items. Grid item - direct descendant of the grid container. Grid line - the dividing lines that make up the structure of the grid. <a href="https://css-tricks.com/snippets/css/complete-guide-grid/">source</a>

## Responsive Images

1. Making images responsive is useful for avoiding art direction probelm

2. srcset allows the browser to choose between multiple images depending onwwhat size the screen is that the page is being viewed on. For example if an image is displayed in its entirety on a computer screen but is cropped and unreadable on a mobile device, srcset allows the browser to pick a smaller version. Size defines the size of the image like the width, which will idicate to the browser which image would be the best option to display. 

3. When the browser loads a page it pre-loads images before the CSS and JS is interpreted which is not ideal for responsive images, so srcset allows the page to pick the version of the image that is best used for the device it's being viewed on. 