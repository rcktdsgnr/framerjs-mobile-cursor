# Mobile Cursor Image for Framer.js

This is a super simple cursor image replacement you can use with your [Framer.js](https://github.com/koenbok/framer) projects, inspired by the one used in the awesome [Framer Studio](http://framerjs.com).

Here's what it looks like: https://dribbble.com/shots/1612931-Cursor-Dribbble

Here's what's needed to make it work on both normal and Retina displays (WebKit only):

```css
html {
	cursor: url('images/cursor.png') 39 39, auto;
	cursor: -webkit-image-set(
		url('images/cursor.png') 1x,
		url('images/cursor@2x.png') 2x
	) 39 39, auto;
}
```
## What to do now?

If you want the cursor to appear in the entire canvas, you can use the code as is. 

If you want to restrict its appearance to a specific area (i.e. only when inside a device mockup) you can change it or move the content of the declaration to a more specific attribute.

Hope you find it useful.

