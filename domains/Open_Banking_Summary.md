---
layout: postSummary
title: Open Banking Articles
description: This is the Open Banking home page with related content 
author: Admin
publishedDate: 1st January 2020
category: [Open Banking]
picture1: image1.png
picture2: image2.png
pictureDir: /images/
permalink: /openbankingsummary
---
<div class="container">
  <br>
  <p class="h5"> {{page.title}}</p>
  <p> {{page.description}} </p>
  {% assign source=site.open_banking %}
  {% include cardlayout.html collection=source %}
  <br>
  <p class="h5">Other related posts</p>
  <p> Blog Posts with Open Banking </p>
  {% assign source=site.posts %}
  {% include cardlayout.html collection=source %}


</div>