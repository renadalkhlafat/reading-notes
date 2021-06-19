# Flash, Video In HTML
HTML5 video is enabled through browser support for video and audio playback, Javascript extensions to control that playback, and ecosystem support for critical functions such as content protection and advertising.  

``` HTML
<video controls>
  <source src="Play.mp4" type="video/mp4">
</video>
```
the most interesting attribute is **CONTROLS**, If this attribute is present, the browser will offer controls to allow the user to control video playback, including volume, seeking, and pause/resume playback.

## The HTMLMediaElement API

provides features to allow you to control video and audio players programmatically. This interface is available to both `<audio>` and `<video>` elements.

``` html
<button class="play" data-icon="P" aria-label="play pause toggle"></button>

<button class="stop" data-icon="S" aria-label="stop"></button>

<button class="rwd" data-icon="B" aria-label="rewind"></button>

<button class="fwd" data-icon="F" aria-label="fast forward"></button>
```

We have four buttons, **play/pause, stop, rewind, and fast forward**. a `data-icon` attribute for defining what icon should be shown on each button.

and an `aria-label` attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags.

## Aligning images Using CSS

*The float property can be used to move an element to the left or the right of its containing block allowing text to flow around it. 

Rather than using the (img) element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

1. The float property is added to the class that was created to represent the size of the image (such as the small class in our example).

2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.