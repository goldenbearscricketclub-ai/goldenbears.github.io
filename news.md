---
layout: default
title: "News & Gallery"
permalink: /news/
---
<section class="page-hero"><p class="eyebrow">FROM THE CLUB</p><h1><span class="lang-en" lang="en">News &amp; Gallery</span><span class="lang-sv" lang="sv">Nyheter och bildgalleri</span></h1><p data-i18n="newsPageIntro">Club updates, training announcements, events and match reports.</p></section>
<section class="section">
{% if site.posts.size > 0 %}
  <div class="cards two">
  {% for post in site.posts %}
    <article class="feature-card">
      <p class="eyebrow">{{ post.date | date: "%d %b %Y" }}</p>
      <h2><a href="{{ post.url | relative_url }}">{% if post.title_sv %}<span class="lang-en">{{ post.title }}</span><span class="lang-sv">{{ post.title_sv }}</span>{% else %}{{ post.title }}{% endif %}</a></h2>
      {% if post.excerpt %}<div class="news-excerpt">{{ post.excerpt }}</div>{% endif %}
      <a href="{{ post.url | relative_url }}"><span class="lang-en">Read update →</span><span class="lang-sv">Läs mer →</span></a>
    </article>
  {% endfor %}
  </div>
{% else %}
  <div class="news-placeholder"><span>📰</span><div><strong data-i18n="newsEmptyTitle">The next club update is coming soon</strong><p data-i18n="newsEmptyText">Add a Markdown post in the _posts folder to publish news here. See the README for instructions.</p></div></div>
{% endif %}
</section>
<section class="section" aria-labelledby="news-gallery-title">
  <h2 id="news-gallery-title">
    <span class="lang-en" lang="en">Photo gallery</span>
    <span class="lang-sv" lang="sv">Bildgalleri</span>
  </h2>
  <div class="news-gallery-grid">
    <div class="news-gallery-placeholder">
      <span class="news-gallery-placeholder-icon" aria-hidden="true">📷</span>
      <p>
        <span class="lang-en" lang="en">Photos from club news and events will appear here.</span>
        <span class="lang-sv" lang="sv">Här visas bilder från föreningens nyheter och evenemang.</span>
      </p>
    </div>
  </div>
</section>
