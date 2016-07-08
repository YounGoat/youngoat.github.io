---
layout: page
title: About
permalink: /about/
autoescape: false
---

YounGoat, borned at the begin of 1980s. He is a coder dreaming of being a programmer. Sometimes he is also a writer.

### Star Me

<div style="clear: both;">
    <style>
        .followme {
            float: left;
            width: 150px;
            height: 100px;
            text-align: center;
            font-style: italic;
            font-size: small;
            border-left: dashed 1px;
            opacity: 0.5;

            -webkit-filter: grayscale(100%);
            -moz-filter: grayscale(100%);
            -ms-filter: grayscale(100%);
            -o-filter: grayscale(100%);
            filter: grayscale(100%);
            filter: gray;
        }

        .followme:hover {
            opacity: 1;
            -webkit-filter: grayscale(0%);
            -moz-filter: grayscale(0%);
            -ms-filter: grayscale(0%);
            -o-filter: grayscale(0%);
            filter: grayscale(0%);
        }
    </style>

    {% for account in site.data.accounts %}
        <a href="{{ account.url }}" target="_blank">
        <div class="followme" style="background: url({{ account.ico }}) 50% 80% no-repeat;">
            {{ account.name }}<br/>@{{ account.site }}
        </div>
        </a>
    {% endfor %}
</div>
