---
layout: default
---

Checkout what our members have been up to! Don't forget to
[Submit your accomplishments][contributing].

<ul class="post-list">
{% assign items = site.items | sort: 'date' %}
{% for post in items reversed %}
  <li>
    <a href="{{ post.link }}" class="post-link">{{ post.title}}</a>
    <span class="post-author">{{ post.author }}</span>
    {% if post.venue %}<span class="post-meta">@ {{ post.venue }}</span>{% endif %}
    {% if post.project %}<span class="post-meta">for {{ post.project }}</span>{% endif %}
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

[contributing]: https://github.com/WriteSpeakCode/accomplishments/blob/gh-pages/CONTRIBUTING.md
