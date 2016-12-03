---
layout: page
title: 你好世界
---
{% include JB/setup %}


<ul>

　　{% for post in site.posts %}

　　　　<li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
            <p> {{ post.content  | | split:'<!--break-->' | first }}</p>

　　{% endfor %}

</ul>