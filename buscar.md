---
layout: page
title: "buscar"
date:
modified:
excerpt:
image:
  feature:
search_omit: true
sitemap: false
---

<!-- Search form -->
<form method="get" action="{{ site.url }}search/" data-search-form class="simple-search">
  <label for="q">Buscar en {{ site.title }}:</label>
  <input type="search" name="q" id="q" placeholder="Què estàs buscant?" data-search-input id="goog-wm-qt" autofocus />
  <input type="submit" value="Buscar" id="goog-wm-sb" />
</form>

<!-- Search results placeholder -->
<h6 data-search-found>
  <span data-search-found-count></span> resultat(s) trobat(s) de &ldquo;<span data-search-found-term></span>&rdquo;.
</h6>
<ul class="post-list" data-search-results></ul>

<!-- Search result template -->
<script type="text/x-template" id="search-result">
  <li><article>
    <a href="##Url##">##Title## <span class="excerpt">##Excerpt##</span></a>
  </article></li>
</script>