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

/* 1) „Untergrund“ der Seite grau */
body { background: #f7f7f8 !important; }

/* 2) Header/Nav bleibt weiß */
.masthead,
.masthead__inner-wrap,
.greedy-nav,
.greedy-nav a,
.greedy-nav__toggle,
.masthead__menu {
  background: #fff !important;
}

/* 3) Content-Wrapper transparent, damit das Grau durchkommt */
.initial-content,
#main,
.page,
.page__inner-wrap,
.page__content,
.archive,
.layout--single {
  background: transparent !important;
}

/* 4) 5% Rand links/rechts im Content */
.page__content{
  padding-left: 5vw !important;
  padding-right: 5vw !important;
}

/* Optional: Footer wieder weiß */
.page__footer,
.page__footer footer {
  background: #fff !important;
}


</style>

<div class="ansatzrechner-wrap">
  <iframe
    src="{{ '/assets/ansatzrechner/index.html' | relative_url }}"
    style="height: calc(100vh - 180px);"
    loading="lazy"
  ></iframe>
</div>
