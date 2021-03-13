---
layout: page
title: art
permalink: /art/
description: a project with a background image test
img: /assets/img/12.jpg
nav: true
importance: 1

description: A growing collection of my favorite art projects.
---

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.

<div class="view overlay">
    <img src="https://mdbootstrap.com/img/Photos/Others/forest-sm.jpg" class="img-fluid " alt="smaple image">
    <div class="mask flex-center rgba-red-strong">
        <p class="white-text">Strong overlay</p>
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/angel1.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/angel2.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/angel3.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>

<div class="caption">
    A sculpture of an angel made with stoneware clay.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/yunior1.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/yunior2.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/yunior3.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>

<div class="caption">
    A superhero made of stoneware clay. Based on Yunior from the "The Brief Wondrous Life of Oscar Wao."
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/search1.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/search2.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/search3.jpeg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>

<div class="caption">
    Stoneware face.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/rock.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/rock1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/rock2.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/rock3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>

<div class="caption">
    Stoneware lantern. Also glazed.
</div>



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>

<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>


<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/" target="_blank">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `` classes.
Here's the code for the last row of images above:

```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded " src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
```
