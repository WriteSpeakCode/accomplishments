---
layout: default
---

Checkout what our members have been up to!

# Write
<ul class="post-list">
{% for post in site.write limit:3 %}
  <li>
    <a href="{{ post.link }}" class="post-link">{{ post.title}}</a>
    <span class="post-author">{{ post.author }} from the {{ post.chapter }} chapter</span>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>

# Speak
<ul class="post-list">
{% for post in site.speak limit:3 %}
  <li>
    <a href="{{ post.link }}" class="post-link">{{ post.title}}</a>
    <span class="post-author">{{ post.author }} from the {{ post.chapter }} chapter</span>
    <span class="post-meta">@ {{ post.venue }} on {{ post.date | date: "%b %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>

# Code
<ul class="post-list">
{% for post in site.code limit:3 %}
  <li>
    <a href="{{ post.link }}" class="post-link">{{ post.title}}</a>
    <span class="post-author">{{ post.author }} from the {{ post.chapter }} chapter</span>
    <span class="post-meta">to {{ post.project }} on {{ post.date | date: "%b %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
