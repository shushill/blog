---
layout: page
title: About
---

A little bit about me !!
> Hi I'm Sushil Verma. 
> 
> I am a Engineer who loves to read and design codes.
> 
> Loves to do problem solving using data structure and algorithm in C++. 
> 
> Currently I'm a R&D Engineer at Synopsys.


<ul>
    {% for post in paginator.posts %}
      <li>
          <h2><a href="">{{ post.title }}</a></h2>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time>
          <p>{{ post.content | strip_html | truncatewords:50 }}</p>
      </li>
    {% endfor %}
</ul>
