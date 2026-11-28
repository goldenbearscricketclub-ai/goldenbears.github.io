---
layout: default
title: "News & Gallery"
seo_title: "Cricket News & Gallery | Golden Bears Järfälla"
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
    <span class="lang-en" lang="en">Photo &amp; video gallery</span>
    <span class="lang-sv" lang="sv">Bild- och videogalleri</span>
  </h2>
  <div class="news-gallery-grid">
    <div class="news-gallery-embed">
      <iframe src="https://www.instagram.com/p/DZmvTXfNGri/embed/" title="Instagram post" loading="lazy" allowfullscreen></iframe>
      <p><a href="https://www.instagram.com/p/DZmvTXfNGri/" target="_blank" rel="noopener noreferrer"><span class="lang-en" lang="en">View on Instagram ↗</span><span class="lang-sv" lang="sv">Se på Instagram ↗</span></a></p>
    </div>
    <div class="news-gallery-embed">
      <iframe src="https://www.instagram.com/p/DcT3GLsOHuf/embed/" title="Instagram post" loading="lazy" allowfullscreen></iframe>
      <p><a href="https://www.instagram.com/p/DcT3GLsOHuf/" target="_blank" rel="noopener noreferrer"><span class="lang-en" lang="en">View on Instagram ↗</span><span class="lang-sv" lang="sv">Se på Instagram ↗</span></a></p>
    </div>
    <div class="news-gallery-embed">
      <iframe src="https://www.instagram.com/p/Dem2Pd5kXtd/embed/" title="Instagram post" loading="lazy" allowfullscreen></iframe>
      <p><a href="https://www.instagram.com/p/Dem2Pd5kXtd/" target="_blank" rel="noopener noreferrer"><span class="lang-en" lang="en">View on Instagram ↗</span><span class="lang-sv" lang="sv">Se på Instagram ↗</span></a></p>
    </div>
  </div>
</section>
