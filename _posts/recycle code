---
layout: post
title: "Recycling codes"
date: 2017-07-11 00:00:01 +0800
categories: jekyll
---
Recycling code using jekyll.
Code reuse, also called software reuse, is a method of programming where you use a existing software or the knowledge of a software, to build a new software - following the reusability principles.

While i was creating the archive I realized postbox was a duplication of the postbox in home.html. So I extracted the postbox into a postbox.html and recycled it on both the home page and the archives page.

```html
{% raw %}
<div class="post-box">
  <div class="post-info">
    <span class="post-date">
      {{ post.date | date: "%B %-d, %Y" }}
    </span>
    <span class="in"> in </span>
    <span class="post-categories">
      {% for category in post.categories %}
      {{category}}
      {% endfor %}
    </span>
  </div>
  <a class="post-title" href="{{post.url | prepend:site.baseurl}}">{{ post.title }}</a>
  <div class="post-excerpt">
    {{ post.content | strip_html | truncatewords:30 }}
  </div>
  </div>
</div>
{% endraw %}
```
