# Bootstrap
Bootstrap is a front-end toolkit that helps you build visually appealing, responsive websites more quickly.   
It provides pre-written **CSS classes**, **JavaScript behavior**, and ready-made components that you can use in your web pages.

## Bootstrap Sample Code
```
<!DOCTYPE html>
<html>

<head>
    <title>Little Lemon</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</head>

<body>
    <div>
        <img src="logo.png" id="logo">
    </div>
    <div class="container">
        <div class="row">
            <div class="col">
                <h1>Our Menu</h1>
                <h2>Falafel <span>NEW</span></h2>
                <p>Chickpea, herbs, spices.</p>
                <h2>Pasta Salad</h2>
                <p>Pasta, vegetables, mozzarella.</p>
                <h2>Fried Calamari</h2>
                <p>Squid, buttermilk.</p>
            </div>
            <div class="col">
                <h2>Prices</h2>
                <table class="table">
                    <tr>
                        <td>Falafel</td>
                        <td>$10</td>
                    </tr>
                    <tr>
                        <td>Pasta Salad</td>
                        <td>$12</td>
                    </tr>
                    <tr>
                        <td>Fried Calamari</td>
                        <td>$15</td>
                    </tr>
                </table>
            </div>
        </div>
    </div>
    <div class="text-center">
        <p>
            Copyright Little Lemon
        </p>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-YvpcrYf0tY3lHB60NNkmxc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
        crossorigin="anonymous"></script>
</body>

</html>
```

## Bootstrap Grid System
The Bootstrap grid helps you divide a page into 12 columns.

```
<div class="row">
    <div class="col-6">Left</div>
    <div class="col-6">Right</div>
</div>
```
Since `6 + 6 = 12`, both boxes take half the row.

### Responsive Grid
One of Bootstrap's biggest strengths is that the layout can change based on screen size.

```
<div class="col-md-6">
```
- On **mobile (<768px)** → the column takes the full width (100%).
- On **medium screens and larger (≥768px)** → it takes **6 out of 12 columns** (50%).
<br>

---
<br>

## Bootstrap Infixes
Infixes are like special labels that tell your website when to change its layout based on the screen size.

```
<div class="col-6 col-lg-2">Menu Item</div>
```
- `col-6` means on extra small screens (default), the column takes up 6 units (half the row width).
- `col-lg-2` means on large screens (≥ 992px), the column takes up 2 units (one-sixth of the row width), so you get 6 columns side by side.
<br>

---
<br>

## Bootstrap Modifiers
In Bootstrap, **modifiers** are like special tags added to CSS classes that change how an element looks or behaves without rewriting the whole style. 

```
<div class="alert alert-primary" role="alert">
  This is a primary alert — it shows in blue.
</div>

<div class="alert alert-danger" role="alert">
  This is a danger alert — it shows in red.
</div>
```
- `alert` is the base class that creates the alert box.
- `alert-primary` is a modifier that colors the alert blue (Bootstrap’s primary color).
- `alert-danger` is another modifier that colors the alert red, indicating an error or danger.
- `role="alert"` helps screen readers understand this is an important message.

<br>

---

<br>

## Spacing Utilities
One of Bootstrap's best features is that you rarely need to write CSS for spacing.
- ### Margin (`m`)
  ```
  <div class="m-3">Content</div>
  ```
  Adds margin on **all sides**.

- ### Padding (`p`)
  ```
  <div class="p-3">Content</div>
  ```
  Adds padding on **all sides**.

### Spacing Scale
Bootstrap uses numbers from 0 to 5.
| Class | Approximate Spacing |
|:---:  |:---:|
|`0`|0|
| `1`|Small|  
|`2`|Medium-Small|
|`3`|Medium|
|`4`|Large|
|`5`|Extra-Large|
