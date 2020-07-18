---
layout: layout.html
---
<h1> Books </h1>

<p>1.HTML and CSS</p>
<p>2.JavaScript and jQuery</p>
<p>3.Head First HTML and CSS</p>
<p>4.Digital Minimalism</p>

<ul>
{%- for post in collections.post reversed -%}
  <li>
    <a href="{{post.url}}">
      {{ post.data.title }}
    </a>
  </li>
{%- endfor -%}
</ul>

