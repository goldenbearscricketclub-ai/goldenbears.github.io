---
layout: default
title: News & announcements
permalink: /news/
---
<section class="page-hero"><p class="eyebrow">FROM THE CLUB</p><h1 data-i18n="newsPageTitle">News & announcements</h1><p data-i18n="newsPageIntro">Club updates, training announcements, events and match reports.</p></section>
<section class="section">
{% if site.posts.size > 0 %}
  <div class="cards two">
  {% for post in site.posts %}
    <article class="feature-card">
      <p class="eyebrow">{{ post.date | date: "%d %b %Y" }}</p>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      {% if post.excerpt %}<p>{{ post.excerpt | strip_html }}</p>{% endif %}
      <a href="{{ post.url | relative_url }}">Read update →</a>
    </article>
  {% endfor %}
  </div>
{% else %}
  <div class="news-placeholder"><span>📰</span><div><strong data-i18n="newsEmptyTitle">The next club update is coming soon</strong><p data-i18n="newsEmptyText">Add a Markdown post in the _posts folder to publish news here. See the README for instructions.</p></div></div>
{% endif %}
</section>
