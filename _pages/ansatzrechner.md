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
  width: 90vw;
  max-width: 90vw;
  margin-left: calc(50% - 45vw);
  margin-right: calc(50% - 45vw);
}

/* 3) Iframe sauber block-level, damit keine komischen Inline-Abstände entstehen */
.ansatzrechner-wrap iframe{
  display: block;
  width: 100%;
  border: 0;
  border-radius: 12px;
}
</style>

<div class="ansatzrechner-wrap">
  <iframe
    src="{{ '/assets/ansatzrechner/index.html' | relative_url }}"
    style="height: calc(100vh - 180px);"
    loading="lazy"
  ></iframe>
</div>


