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
    {% for links in paginator.posts %}
      <li>
          <h2><a href="{{ links.url | prepend: site.baseurl | replace: '//', '/' }}">{{ links.title }}</a></h2>
      </li>
    {% endfor %}
</ul>
