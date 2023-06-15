---
layout: home
---

<main class="home archive">

<article class="post">

<header>

<div class="introblock">
<p>
  Hi, I'm William (sometimes Bill), I live on <a href="">Sydneys' Northern Beaches</a>,
  where I enjoy <a href="">running</a>, <a href="">swimming</a>, and
  <a href="">slowly making things in my workshop</a>.
</p>
<p>
  I have been interested in <a href="">music</a>, <a href="">alternative lifestyles</a> and <a href="">technology</a> since the <a href="">70's</a>.
</p>
<p>
  Enjoyed stints as a <a href="">protester</a>, <a href="">natural therapist</a>, and spent most of my career has been working in <a href="https://www.linkedin.com/in/williampickup/">IT</a>.
</p>
<p>
You can find my occasionally updated blog <a href="https://social.williampickup.org">here</a>
</p>
<p>
  For More about me see <a href="/about.html">my “about” page</a>.
</p>
<h2>
  What am I doing now?
</h2>
<p>
  See <a href="/now.html">my “now” page</a>
</p>
<h2>
  Contact me
</h2>
<p>
<a href="/contact.html">say hello</a>
</p>
</div>

</header>

<h2>Latest posts</h2>
<small><a href="{{ '/posts' | relative_url }}">See All Posts</a></small>

{% assign counter = 0 %}

<ul>
  {% for post in collections.posts.resources %}
  {% assign counter = counter | plus: 1 %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a>
    </li>
    {% if counter == 3 %} {% break %} {% endif %}
  {% endfor %}
</ul>
