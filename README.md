#Vertically Align Block Elements

##Flexbox
The CSS3 Flexible Box, or flexbox, is a layout mode providing for the arrangement of elements on a page such that the elements behave predictably when the page layout must accommodate different screen sizes and different display devices.
```css
.parent {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
```

http://codepen.io/chriscoyier/pen/FqDyi

##Unknown Height
This method words by shifting the top of the element down 50% of its parent's height, and then pushing it up half of it's own height.
```css
.parent {
  position: relative;
}
.child {
  position: absolute;
  top: 50%;
  transform: translateY(50%);
}
```

http://codepen.io/chriscoyier/pen/lpema

##Known Height
If you must, you can also center with pixels if the height of your element is known and fixed.

```css
.parent {
  position: relative;
}
.child {
  position: absolute;
  top: 50%;
  height: 100px;
  margin: -50px;
}
```

http://codepen.io/chriscoyier/pen/HiydJ
