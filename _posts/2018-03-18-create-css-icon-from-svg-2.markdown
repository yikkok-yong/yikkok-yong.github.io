---
layout: post
title:  "Create CSS Icon from SVG - Part 2"
date:   2018-03-18 10:00:00 +0800
categories: icon svg css
author: John Yong
excerpt_separator: <!--Read More...-->
published: false
---

How to include font in CSS...
<br>
This post is record about how to use the svg font in CSS
<!--Read More...-->

## Steps: Using font in CSS
------

1. Create a new CSS file - "font.css"
> Write the following to your css file
```css
   @font-face {
       font-family: 'MyFont';
       src: url('path/to/your/Font.ttf') format('truetype');
       font-weight: normal;
       font-style: normal;
   }
```

2. Then, continue with below code:
> The purpose for this class is to create a namespacing
```css
    .my-font {
        font-family: 'MyFont' !important;
        /* and other default config for this class, such as font-weight, size or others */
    }
```

3. Create class for each of your svg font:
```css
    .my-font.icon-pokeball::before {
        /* ---
         * The unicode can be obtain from fontforge
         * unicode that mapped to the svg you allocated.
         * For this case, I picked the "plus" symbol
         * and its unicode is U+002b
         * ---
         */
        content: '\002b';
    }
```

4. Now, include the "font.css" to any web project, to use the svg font:
```html
    <span class="my-font icon-pokeball"></span>
```

5. [Here is the link for the source]({{relative_path}}/assets/source/create-icon-from-svg.zip)