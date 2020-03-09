---
layout: page
title: "TEST"
permalink: /test/a
list: <% _.forEach(people, function(name) { %><li><%= name %></li><% }); %>
people:
- Jon Schlinkert
- Brian Woodward
---



<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>{{title}}</title>
  </head>
  <body>
    <section class="people">
      <ul>
        {{{list}}}
      </ul>
    </section>
  </body>
</html>