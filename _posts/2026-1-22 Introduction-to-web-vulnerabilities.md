############################################
# _config.yml
############################################
title: Web Security Blog
description: Learning Web Vulnerabilities
theme: minima
permalink: /:categories/:title/
markdown: kramdown

############################################
# _layouts/default.html
############################################
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>{{ page.title }}</title>
</head>
<body>

<nav>
  <a href="/">Home</a> |
  <a href="/categories.html">Categories</a> |
  <a href="/tags.html">Tags</a>
</nav>
<hr>

{{ content }}

</body>
</html>

############################################
# _layouts/post.html
############################################
---
layout: default
---

<h1>{{ page.title }}</h1>
<p><small>{{ page.date | date: "%B %d, %Y" }}</small></p>

<p>
Category: {{ page.categories }} |
Tags: {{ page.tags | join: ", " }}
</p>

<hr>
{{ content }}

############################################
# index.html  (HOME)
############################################
---
layout: default
title: Home
---

<h1>Latest Posts</h1>

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a><br>
    <small>
      Category: {{ post.categories }} |
      Tags: {{ post.tags | join: ", " }}
    </small>
  </li>
{% endfor %}
</ul>

############################################
# categories.html
############################################
---
layout: default
title: Categories
---

<h1>Categories</h1>

{% for category in site.categories %}
  <h2>{{ category[0] }}</h2>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

############################################
# tags.html
############################################
---
layout: default
title: Tags
---

<h1>Tags</h1>

{% for tag in site.tags %}
  <h2>{{ tag[0] }}</h2>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

############################################
# _posts/2026-01-22-introduction-to-sql-injection.md
############################################
---
layout: post
title: "Introduction to SQL Injection"
date: 2026-01-22
categories: web-development
tags:
  - sql-injection
  - web-security
---

## Introduction

SQL Injection (SQLi) is a critical web vulnerability that allows attackers to interfere with database queries by injecting malicious SQL code through user input.

## Vulnerable Example

```sql
SELECT * FROM users WHERE username = '$username' AND password = '$password';
