# 🦖 Dino Design CSS Framework 🦕  <a name="-dino-design-css-framework---"></a>
*Elevate your project's visual aesthetics by easy integrating with Dino Design, an open-source CSS framework.*

<br />

### Table of Contents <a name="table-of-contents-"></a>

- [🦖 Dino Design CSS Framework 🦕  ](#-dino-design-css-framework---)
    - [Table of Contents ](#table-of-contents-)
  - [🚀 Get Started with Dino Design ](#-get-started-with-dino-design-)
    - [Step 1: Download the Stylesheet ](#step-1-download-the-stylesheet-)
    - [Step 2: Include in Your Project ](#step-2-include-in-your-project-)
  - [📝 Usage Guide - Utilities ](#-usage-guide---utilities-)
    - [1. Font Family ](#1-font-family-)
    - [2. Typography ](#2-typography-)
    - [3. Colors ](#3-colors-)
    - [4. Margin \& Padding ](#4-margin--padding-)
    - [5. Borders ](#5-borders-)
  - [📝 Usage Guide - Elements ](#-usage-guide---elements-)
    - [1. Buttons ](#1-buttons-)
    - [2. Tables ](#2-tables-)
    - [3. List ](#3-list-)
    - [4. Form \& Input ](#4-form--input-)
  - [🎨 Customization ](#-customization-)

<br />

## 🚀 Get Started with Dino Design <a name="-get-started-with-dino-design-"></a>

### Step 1: Download the Stylesheet <a name="step-1-download-the-stylesheet-"></a>
[Download the main.css](css/main.css) to kickstart your project's aesthetic appeal.

### Step 2: Include in Your Project <a name="step-2-include-in-your-project-"></a>
Once downloaded, integrate Dino Design into your project by adding the following link to the `<head>` of your HTML document:

```html
<link rel="stylesheet" href="css/main.css">
```
💡 Make sure to adjust the href path according to your project structure.


*Now, you're ready to elevate your project's visual aesthetics!*

<br />

## 📝 Usage Guide - Utilities <a name="-usage-guide---utilities-"></a>

### 1. Font Family <a name="1-font-family-"></a>
For the Dino Design brand, we utilize the sans-serif font Fredoka, accessible via [Google fonts](https://fonts.google.com/specimen/Fredoka).

Incorporate the `$font-stack` variable into your stylesheet in the class or tag you desire, as illustrated below in the body tag:


```scss
body {
    font-family: variables.$font-stack;
}
```

<br />

### 2. Typography <a name="2-typography-"></a>
The typography is defined in the `_typography.scss` file as outlined below.

> **Font Weight Variables:** These variables allow you to control the thickness of the text, providing flexibility in conveying hierarchy and emphasis.
```scss
$fs-sm: 0.8rem; // Small font size
$fs-md: 1rem; // Medium font size
$fs-lg: 1.5rem; // Large font size
$fs-xl: 2rem; // Extra-large font size
$fs-xxl: 2.5rem; // Extra-extra-large font size
```

> **Font Size Variables:** These variables enable you to set consistent and responsive text dimensions throughout your project.

```scss
$fw-light: 300; // Light font weight
$fw-regular: 400; // Regular font weight
$fw-medium: 500; // Medium font weight
$fw-semibold: 600; // Semibold font weight
$fw-bold: 700; // Bold font weight
```

Incorporate the font sizes and weights variables:
- into your `css` stylesheet

```scss
 /* Utilize the 'typography' prefix for accessing values defined in the corresponding file */
body {
    font-size: typography.$fs-md;
    font-weight: typography.$fw-regular;
}
```

- directly within a tag in your `html` file using the class attribute

```html
<h1 class="fs-md fw-regular"><h1>
```

<br />

### 3. Colors <a name="3-colors-"></a>

<br />

### 4. Margin & Padding <a name="4-margin--padding-"></a>
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
```scss
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

<br />

### 5. Borders <a name="5-borders-"></a>
Borders are easily customized through variables.scss. <br>Edit the following variables to match your design preferences:

under variables.scss  
```scss
$table-border-color: #cccccc; 
```
Change this to customize border color,<br>
After adjustments, recompile Sass to update main.css with your new settings.

<br />

## 📝 Usage Guide - Elements <a name="-usage-guide---elements-"></a>

### 1. Buttons <a name="1-buttons-"></a>
*(temporary notes)*
<br />
Dino has a base `.btn` class that sets up basic styles such as size and padding. By default, `.btn` controls have a transparent border and primary background color, without any effects such as hover effect.
<br />
Button variants includes outline, light and dark.

```html
<button type="button" class="btn btn-outline">Outline</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>
```

<br />

### 2. Tables <a name="2-tables-"></a>
To apply custom styling to tables, ensuring clarity and visual appeal, use the class mt-1 for a standardized look:

```html
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
```

<br />

### 3. List <a name="3-list-"></a>

<br />

### 4. Form & Input <a name="4-form--input-"></a>


<br />

## 🎨 Customization <a name="-customization-"></a>