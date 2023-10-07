# SOLUTION

## Z-INDEX
Z Index (z-index) is a CSS property that defines the order of overlapping HTML elements. Elements with a higher index will be placed on top of elements with a lower index.

Note: Z index only works on positioned elements (`position:absolute`, `position:relative`, or `position:fixed`).


### **Some Key Points :**
- If two elements have the same `z-index` value, the element placed last in html code will appear on top of the element placed before it in the code.
- Elent with a higher `z-index` value will appear on top of elements with lower vaalues.
- `Z-index` will have no effect on static elements. It only works for positioned elements.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
   
</head>
<body>
    <div class="container">
        <div class="box" id="blue"></div>
        <div class="box" id="red"></div>
        <div class="box" id="green"></div>
    </div>
</body>
</html>
```

```css
 .container{
            position: relative;
        }
        .box{
           height: 100px;
           width: 100px;
           border: 2px solid black;
        }

        #blue{
            background-color: blue;
            z-index: 2;
            position: absolute;
        }

        #red{
            background-color: red;
            z-index: 1;
            position: absolute;
        }

        #green{
            background-color: green;
            z-index: 3;
            position: absolute;
        }
```