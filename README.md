# Dino Design CSS Framework
<!-- Description -->


## Get Started

To include Dino Design in your project, add the following link to the `<head>` of your HTML document:

```html
<link rel="stylesheet" href="css/main.css">
```
Adjust the `href` path to fit your project structure.

### Usage - Utilities

#### Font

#### Colors

#### Margin & Padding
*(Notation)*
<br />
Property is one of:
- m - for classes that set margin
- p - for classes that set padding

Sides is one of:
- t - for classes that set margin-top or padding-top
- b - for classes that set margin-bottom or padding-bottom
- s - (start) for classes that set margin-left or padding-left
- e - (end) for classes that set margin-right or padding-right
- x - for classes that set both *-left and *-right
- y - for classes that set both *-top and *-bottom
- blank - for classes that set a margin or padding on all 4 sides of the element

Size is one of:
- 0 - for classes that eliminate the margin or padding by setting it to 0
- sm - (by default) for classes that set the margin or padding to rem * .0.2
- md - (by default) for classes that set the margin or padding to rem * .0.8
- lg - (by default) for classes that set the margin or padding to rem * 1.5

(You can change sizes by amending entries to the $variables Sass map variable.)

> Examples
```
.m-0 {
    margin: variables.$m-0;
}
.mx-lg {
    margin-left: variables.$ms-lg;
    margin-right: variables.$ms-lg;
}
.py-md {
    padding-top: variables.$ps-md;
    padding-bottom: variables.$ps-md;
}
```


#### Borders
Borders are easily customized through variables.scss. <br>Edit the following variables to match your design preferences:

under variables.scss  
```
$table-border-color: #cccccc; 
```
Change this to customize border color,<br>
After adjustments, recompile Sass to update main.css with your new settings.

### Usage - Elements

#### Buttons
*(temporary notes)*
<br />
Dino has a base `.btn` class that sets up basic styles such as size and padding. By default, `.btn` controls have a transparent border and primary background color, without any effects such as hover effect.
<br />
Button variants includes outline, light and dark.

```
<button type="button" class="btn btn-outline">Outline</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>
```

#### Tables
To apply custom styling to tables, ensuring clarity and visual appeal, use the class mt-1 for a standardized look:

````
<table class="mt-1">
    <tr>
        <th>Name</th>
        <th>Email</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>John Doe</td>
        <td>johndoe@example.com</td>
        <td>28</td>
    </tr>
    <tr>
        <td>Jane Smith</td>
        <td>janesmith@example.com</td>
        <td>32</td>
    </tr>
</table>
````

#### List

#### Form & Input


### Customization