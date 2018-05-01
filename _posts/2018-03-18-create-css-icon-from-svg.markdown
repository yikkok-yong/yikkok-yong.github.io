---
layout: post
title:  "Create CSS Icon from SVG - Part 1"
date:   2018-03-18 10:00:00 +0800
categories: icon svg css
author: John Yong
excerpt_separator: <!--Read More...-->
published: false
---

How to create css icon from svg file...
<!--Read More...-->

<br />

## Tools
------

1. [Inkscape](https://inkscape.org/en/)
> An open source vector graphics editor, to create a svg file for this case.

2. [FontForge](https://fontforge.github.io/en-US/)
> An open source font editor, to create font from svg.

## Steps: Turn svg into font (.ttf)
------

1. Open fontforge and choose a folder, then click "new"
<img src="{{relative_url}}/assets/images/blog/20180318/fontforge_create_new_font.png" alt="Choose a folder" class="img-fluid" />

2. Select an available symbol, and double click
<img src="{{relative_url}}/assets/images/blog/20180318/pick_one.png" alt="Pick an available symbol" class="img-fluid" />

3. FontForge will prompt a sub window, for create/edit/import font. For this case, I'm going to import a svg file.
<img src="{{relative_url}}/assets/images/blog/20180318/select_import.png" alt="Import a svg file" class="img-fluid" />

4. Now, navigate to ```element > Font Info```, you may do this on FontForge's sub window or main window.
> Fill in three fields:
> * Font Name
> * Font Family Name
> * Name For Human
<img src="{{relative_url}}/assets/images/blog/20180318/select_font_info.png" alt="Fill in necessary info" class="img-fluid" />

5. Then, navigate to ```File > generate font```, select "truetype (.ttf)", click "Ok"

6. To be Continue... [Create CSS Icon from SVG - Part 2]({% post_url 2018-03-18-create-css-icon-from-svg-2 %})