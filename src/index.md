---
layout: page
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
</header>

<h2>Latest posts</h2>
<small><a href="<% relative_url '/posts' %>">See All Posts</a></small>

<ul>
ul>
  <% collections.posts.resources[0..5].each do |post| %>
    <li>
      <a href="<%= post.relative_url %>"><%= post.data.title %></a>
    </li>
  <% end %>
</ul>
