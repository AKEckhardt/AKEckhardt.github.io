---
title: "Ansatzrechner"
permalink: /ansatzrechner/
layout: single
author_profile: false
sidebar: false
---

<style>
/* Jekyll-Titel ausblenden */
.page__title, h1.page__title { display: none !important; }

/* Theme-Container auf dieser Seite „entklemmen“ */
.page,
.page__inner-wrap,
.initial-content,
.page__content {
  max-width: none !important;
  width: 100% !important;
}

/* 5% Rand links/rechts */
.page__content {
  padding-left: 5vw !important;
  padding-right: 5vw !important;
}

/* Iframe */
.ansatz-iframe{
  display:block;
  width:100%;
  height: calc(100vh - 180px);
  border:0;
  border-radius:12px;
}
</style>

<iframe
  class="ansatz-iframe"
  src="{{ '/assets/ansatzrechner/index.html' | relative_url }}"
  loading="lazy"
></iframe>
