# semantics-and-accessibility


# Overview
This is my submission for my first Bootcamp Challenge Assignment. I improved the accessibility of this website by improving the existing codebase in the following ways:
- Replaced general html tags such as `<div>` with specific tags such as `<nav>`
- Added CSS and HTML comments
- Added `alt` attributes to images
- Consolidated redundant classes and CSS rules

# Purpose
The purpose of this website to provide Horiseon's customers with information about their services.

# Changes to HTML semantic structure
The original code exclusivly used `<div>` elements with unique classes to wrap each section with a header, photo, and paragragh in the main body of the website now called `<div class="content">`. This meant while each of those three sections were styled exactly the same, the CSS to define their styling was duplicated for each of the three sections. I removed the unique class names and replaced the `<div>` elements with `<section>` elements, then defined the styling for a `<section>` element in the parent class `content`.

For example:
```css
.content section {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: `Gill Sans`, `Gill Sans MT`, Calibri, `Trebuchet MS`, sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
```

I used this technique to rename the `<aside>` section and consolidate the CSS needed to define its styling too.

# Roadmap
While improving the responsivness of this website and adding features such as CSS animations are outside of the scope of this version of the website, I hope to make these improvements later on.
