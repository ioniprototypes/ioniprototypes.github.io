---
layout: home
title: Home Page
author: Admin
publishedDate: 1st January 2020
category: Home
picture1: image1.png
picture2: image2.png
picture3: none
pictureDir: /images/
figureCaption: IONI Image
permalink: /home
brandPhrase: Connecting People with Data and Technology
---
<div class="container">
<!--Start of IONI Services Currently Offered-->
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in site.orgservices %}
      <div class="col mb-4">
        <div class="card">
          <div class="card-header text-center">
            <a href="{{ item.url }}">
              <figure class="figure">
                <img src="{{site.url}}{{item.pictureDir}}{{item.picture1}}" class="figure-img img-fluid" alt="{{item.figureCaption}}" width="70%">
              <figcaption class="figure-caption text-right">{{item.figureCaption}}</figcaption>
              </figure>
            </a>
          </div>
          <div class="card-body">
            <p class="text-info"> {{item.displayCategory}}</p>
            <a href="{{ item.url }}">
              <h5 class="card-title"> {{item.title}}</h5>
            </a>
            <p class="card-text">{{ item.excerpt }}</p>
            <p class="card-text"><small class="text-muted">Last updated {{item.publishedDate }}</small></p>
            <p class="card-text">Contact to find out how IONI can help>> </p>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
  <!--End of IONI Services Currently Offered-->
  <hr>
    <p class="h3"> Latest Activity </p>
  <hr>
  <!--Start of latest blog activity-->
  <div class="row row-cols-1 row-cols-md-3">
    {% for item in site.posts %}
      <div class="col mb-4">
        <div class="card">
          <div class="card-header">
            <p class="text-info"> {{item.displayCategory}}</p>
            <h5 class="card-title"> {{item.title}}</h5>
          </div>
          <div class="card-body">
              <a href="{{ item.url }}">
                <img src="{{site.url}}{{item.pictureDir}}{{item.picture1}}" class="card-img-top" alt="{{item.picture1Description}}">
              </a>
            <p class="card-text">{{ item.excerpt }}</p>
            <p class="card-text"><small class="text-muted">Last updated {{item.publishedDate }}</small></p>
            <p class="card-text">Contact to find out more >> </p>
            <a>
              <img src= "/images/icon-small.png" width="40" height="40" alt="IONI"> 
              Author: {{item.author}}
            </a>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
  <!-- end of Bloging Activity -->
 </div>
  

