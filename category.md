---
layout: blog
title: "Category List"
permalink: /category/
---

<header>
    <h1>Kategori Ceritanya</h1>
</header>

<ul class="tag-box inline">
{% assign list = site.tags | sort %}
    {% for category in list %}
        <li>
            <a href="#{{ category[0] }}">
                {{ category[0] }}
            </a>
            <span>({{ category[1].size }})</span>
        </li>
    {% endfor %}
{% assign list = nil %}
</ul>
{% endfor %}
{% assign taglist = nil %}
