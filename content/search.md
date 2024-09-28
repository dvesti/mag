---
title: Поиск
weight: 5
menu: [main, top]
---

<style type="text/css">
#search-input {
  width: 100%;
  font-size: 1.2em;
  padding: .5em;
}
.search-results {
  font-size: .9em;
}
.search-results b {
  background-color: yellow;
}
</style>

The search is performed via fuse.js. For the search keywords, white spaces act as the `AND` operator, and `|` acts as the `OR` operator. To match an exact phrase, double quote it. For example, `R Markdown` matches articles that contain both `R` and `Markdown`, `R | Markdown` matches articles that contain `R` or `Markdown`, and `"R Markdown"` matches articles that contain the whole phrase `R Markdown`.

<input type="search" id="search-input" data-info-init="Искать……" data-info-ok="Найдено：" data-info-fail="Не найден файл поиска！">

<div class="search-results">
<section>
<h2><a target="_blank"></a></h2>
<div class="search-preview"></div>
</section>
</div>

<script src="https://cdn.jsdelivr.net/npm/fuse.js@6.6.2" defer></script>
<script src="https://cdn.jsdelivr.net/npm/@xiee/utils/js/fuse-search.min.js" defer></script>
