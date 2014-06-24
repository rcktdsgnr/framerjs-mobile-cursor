# Mobile Cursor Image 

This is a super simple cursor image replacement you can use with [framer.js](https://github.com/koenbok/framer) base template, inspired by the one used in the iOS simulator and the super cool [Framer Studio](http://framerjs.com)..

Here's what's needed to make it work on both normal and Retina displays:

```css
html {
	cursor: url('images/cursor.png') 30 30, auto;
	cursor: -webkit-image-set(
		url('images/cursor.png') 1x,
		url('images/cursor@2x.png') 2x
	) 30 30, auto;
}
```

If you want the cursor to appear in the entire canvas, you can use the code as is. 

If you want to restrict its appearance to a specific area (i.e. only when inside a device mockup) you can change it or move it to a more specific attribute.

Hope you find it useful.

