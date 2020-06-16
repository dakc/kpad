# kpad
javascript library for sketchpad using canvas.
kpad will create a canvas inside given DOM element.

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>kPad</title>
    <style>
        body{
            margin: 0px;
            padding: 0px;
        }
        .sign {
            width: 100%;
            height: 100vh;
        }
    </style>
</head>

<body>

    <div class="sign"></div>

    <script src="kpad.min.js"></script>

    <script>
        const options = {
            colors: ["red", "blue", "pink"],
        };
        const parentElement = document.querySelector(".sign");
        new kpad(parentElement, options);
    </script>
</body>

</html>
```
