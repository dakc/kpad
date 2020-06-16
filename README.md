# kpad
javascript library for creating sketchpad using canvas.


## usage
kpad will create a canvas inside given DOM element.
By setting the size of outer element, we can easily manipulate different size of canvas.
```javascript
const parentElement = document.querySelector(".sign");
new kpad(parentElement);
```

## pen color
By passing "colors" which is simply arrays of color as option, we can use various types of pen.It will show a control box which is draggable and can be moved to any place at any time.
```javascript
const parentElement = document.querySelector(".sign");
const options = {colors: ["red", "yellow", "blue"]}
new kpad(parentElement, options);
```

## options
We can pass following additional parameter as per our need.
```javascript
const parentElement = document.querySelector(".sign");
const options = {
    colors: ["red", "yellow", "blue"] // users will be able to chose 3 different pens
    backgroundColor: "green", // background color of sketchpad, default is white
    size: 5, // width of the pen, default is 1
    color: "black", // pen color, default is red
    sizeIncreement: 10, // size by which pen width will be increased or decreased, default is 2
};
new kpad(parentElement, options);
```
## sample
see here for [sample page](./sample.html).

# Demo
see here for [DEMO](https://dakc.github.io/kpad/sample.html)

# lisence
MIT