# kpad
javascript library for sketchpad using canvas.


## usage
kpad will create a canvas inside given DOM element.
By setting the size of outer element, we can easily manipulate different size of canvas.
```javascript
const parentElement = document.querySelector(".sign");
new kpad(parentElement);
```

## pen color
It will show a control box show that user can select various coloured pen.
```javascript
const parentElement = document.querySelector(".sign");
const options = {colors: ["red", "yellow", "blue"]}
new kpad(parentElement, options);
```

## options
```javascript
const parentElement = document.querySelector(".sign");
const options = {
    colors: ["red", "yellow", "blue"] // users will be able to chose 3 different pens
    backgroundColor: "green", // background color of sketchpad, default is white
    size: 5, // width of the pen, default is 2
    color: "black", // pen color, default is red
    sizeIncreement: 10, // size by which pen width will be increased or decreased
};
new kpad(parentElement, options);
```
## sample
see here for [sample page](./sample.html).

# lisence
MIT