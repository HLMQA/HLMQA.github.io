---
layout: page
title: About me
permalink: /about/
sidebar: true
---


**Education**

<div class="archive">
  <div class="timeline" id="timeline">
    {% for career in site.data.index.careers %}
          <div class="archive-title"><div class="archive-year"><strong>{{ career.date }}</strong> {{ career.job }} @ <a href="{{ career.link }}">{{ career.name }}</a></div></div>
    {% endfor %}
  </div>
</div>

<div class="navy-line"></div>

**Community involvement**

<div class="archive">
  <div>
    {% for career in site.data.index.academic %}
         <div ><div ><strong>{{ career.date }}</strong> {{ career.job }} 
          {% if career.link %}
              <a href="{{ career.link }}">{{ career.name }}</a>
          {%else %}
              {{ career.name }}
          {% endif %}
          </div></div>
    {% endfor %}
  </div>
</div>

**Languages**

- **Moroccan Darija** - native
- **English** - proficient
- **French** - proficient
- **Arabic** - proficient
- **Portuguese** - fluent