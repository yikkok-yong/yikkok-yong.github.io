---
layout: page
title: About
permalink: /about/
---

<div class="justify-content-around">
    <ul class="nav nav-tabs about-me" role="tablist">
        <li role="presentation" class="nav-item"><a href="#me" class="nav-link active" aria-controls="me" role="tab" data-toggle="tab">About Me</a></li>
        <li role="presentation" class="nav-item"><a href="#site" class="nav-link" aria-controls="site" role="tab" data-toggle="tab">About This Site</a></li>
    </ul>
    <div class="tab-content">
        <div role="tabpanel" class="tab-pane active" id="me">
            <div class="p-3">
                {% include personal/aboutme.html %}
            </div>
        </div>
        <div role="tabpanel" class="tab-pane" id="site">
            <p class="lead pt-3">This site were build by and credit to: </p>
            <ul>
                <li><a href="https://pages.github.com/">GitHub Pages</a></li>
                <li><a href="https://jekyllrb.com/">Jekyll</a></li>
                <li><a href="https://getbootstrap.com/docs/4.0/getting-started/introduction/">Bootstrap 4</a></li>
                <li><a href="https://fonts.google.com/specimen/Josefin+Slab">Font family: Josefin Slab</a></li>
                <li><a href="https://openclipart.org/detail/12979/lemon">Favicon</a></li>
            </ul>
        </div>
    </div>
</div>