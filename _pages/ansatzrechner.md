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

/* Hintergrundfarbe der ganzen Seite (außer evtl. Theme-Header) */
body { background: #f7f7f8 !important; }

/* Minimal Mistakes / typische Wrapper: sorgt dafür, dass wirklich alles grau ist */
.page,
.initial-content,
.page__inner-wrap,
.page__content,
.archive {
  background: transparent !important;
}

/* Optional: falls der Theme-Header/Nav noch weiß ist und du ihn auch grau willst */
.masthead,
.greedy-nav,
.masthead__inner-wrap {
  background: #f7f7f8 !important;
}


</style>

<div class="ansatzrechner-wrap">
  <iframe
    src="{{ '/assets/ansatzrechner/index.html' | relative_url }}"
    style="height: calc(100vh - 180px);"
    loading="lazy"
  ></iframe>
</div>
