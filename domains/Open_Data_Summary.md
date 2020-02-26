---
layout: postSummary
title: Open Data Articles
description: Open Data Items
author: Admin
publishedDate: 1st January 2020
category: [Open Data]
categoryDisplay : Open data
picture1: image1.png
picture2: image2.png
pictureDir: /images/
permalink: /opendatasummary
author: Jonathan Silvester
---
<div class="container">
  <br>
  <p class="h5"> {{page.title}}</p>
  <p> {{page.description}} </p>
  {% assign source=site.data_catalogue %}
  {% include cardlayout.html collection=source %}
  <br>
  <p class="h5">Other related posts</p>
  <p> Open Data blog posts </p>
  {% assign source=site.posts %}
  {% include cardlayout.html collection=source %}
</div>