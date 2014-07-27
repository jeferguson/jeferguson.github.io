---
layout: default_home
permalink: /blog/
---


<!-- might need to rearrange the row placing later-->

<ul class="posts">
    {% for post in site.posts %}

    <div class ="row">
      <div class="large-1 columns"></div>
      <div class="large-11 columns">

          <li>
            <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>            
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
                          <p>{{ post.line }}</p>
            
          </li>
      </div>
    </div>

    {% endfor %}
</ul>
  
