---
layout: default
---

# Accomplishments
Checkout what our members have been up to!

## Write
{% for post in site.write limit:3 %}
* [{{ post.title}}]({{ post.link }})

    {{ post.author }} from the {{ post.chapter }} chapter

    {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}

## Speak
{% for post in site.speak limit:3 %}
* [{{ post.title}}]({{ post.link }})

    @ {{ post.venue }}

    {{ post.author }} from the {{ post.chapter }} chapter

    {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}

## Code
{% for post in site.code limit:3 %}
* [{{ post.title}}]({{ post.link }})

    {{ post.author }} from the {{ post.chapter }} chapter

    {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}
  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
