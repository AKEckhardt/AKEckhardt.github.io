---
title: "Ansatzrechner"
permalink: /ansatzrechner/
layout: single
author_profile: false
sidebar: false
classes: wide
---

<style>
/* 1) Jekyll/Theme-Überschrift (page title) auf dieser Seite ausblenden */
.page__title { display: none !important; }

/* 2) Iframe-Container: 90% der Viewportbreite (= 5% Rand links/rechts),
      zentriert und unabhängig vom Theme-Container */
.ansatzrechner-wrap{
  width: 94vw;
  max-width: 94vw;
  margin-left: calc(50% - 48.5vw);
  margin-right: calc(50% - 45.5vw);
}

/* 3) Iframe sauber block-level, damit keine komischen Inline-Abstände entstehen */
.ansatzrechner-wrap iframe{
  display: block;
  width: 100%;
  border: 0;
  border-radius: 12px;
}

/* Header/Nav explizit weiß lassen */
body { background: #fff !important; }
.masthead,
.masthead__inner-wrap,
.greedy-nav,
.greedy-nav a,
.greedy-nav__toggle,
.masthead__menu {
  background: #fff !important;
}

/* NUR der Inhaltsbereich (unter dem Header) soll grau sein */
.initial-content {
  background: #f7f7f8 !important;
}

/* Die inneren Boxen sollen transparent sein, damit das Grau durchscheint */
.page,
.page__inner-wrap,
.page__content,
.archive {
  background: transparent !important;
}


</style>

<div class="ansatzrechner-wrap">
  <iframe
    src="{{ '/assets/ansatzrechner/index.html' | relative_url }}"
    style="height: calc(100vh - 180px);"
    loading="lazy"
  ></iframe>
</div>
