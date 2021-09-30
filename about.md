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


<section>
  {% if site.posts[0] %}

  

    {%for post in site.posts %}
      {% unless post.next %}
          <h3>{Hello}</h3>
          <ul>
        {% endif %}
      {% endunless %}
        <li><time>{{ post.date | date:"%d %b" }} - </time>
          <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
            {{ post.title }}
          </a>
        </li>
    {% endfor %}
    </ul>

  {% endif %}
</section>
