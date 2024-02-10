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