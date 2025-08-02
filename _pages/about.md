---
permalink: /
title: "Hi"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!DOCTYPE html>
<html lang="en">
  <head>
    {% include head.html %}
  </head>
  <body>
    {% include header.html %}

    <div class="container mt-4">
      <div class="row">
        <div class="col-md-8">
          <h1>{{ page.title }}</h1>
          <p>Welcome to my academic homepage.</p>
          <p>I am an undergraduate student with interest in computer architecture, compilers, and formal verification.</p>
          <p>Use the navigation bar above to browse my <a href="/publications/">publications</a>, <a href="/teaching/">teaching</a>, and <a href="/projects/">projects</a>.</p>
        </div>

        <div class="col-md-4">
          {% if page.author_profile %}
            {% include author-profile.html %}
          {% endif %}
        </div>
      </div>
    </div>

    {% include footer.html %}
  </body>
</html>
