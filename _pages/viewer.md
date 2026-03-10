---
title: ""
permalink: /viewer/
layout: single
author_profile: false
sidebar: false
classes: wide
---

<style>
  .page__title { display: none !important; }

  body {
    background: #f7f7f8 !important;
  }

  .masthead,
  .masthead__inner-wrap,
  .greedy-nav,
  .greedy-nav a,
  .greedy-nav__toggle,
  .masthead__menu {
    background: #fff !important;
  }

  .initial-content,
  #main,
  .page,
  .page__inner-wrap,
  .page__content,
  .archive,
  .layout--single {
    background: transparent !important;
  }

  .page__content {
    padding-left: 0 !important;
    padding-right: 0 !important;
    max-width: none !important;
  }

  .viewer-wrap {
    width: 100vw;
    max-width: 100vw;
    margin-left: calc(50% - 50vw);
    margin-right: calc(50% - 50vw);
  }

  .viewer-wrap iframe {
    display: block;
    width: 100%;
    min-height: calc(100vh - 140px);
    border: 0;
    border-radius: 0;
  }

  .page__footer,
  .page__footer footer {
    background: #fff !important;
  }
</style>

<div class="viewer-wrap">
  <iframe
    id="viewer-frame"
    src="{{ '/assets/viewer/index.html' | relative_url }}"
    loading="lazy">
  </iframe>
</div>

<script>
  function resizeViewerFrame() {
    const iframe = document.getElementById("viewer-frame");
    if (!iframe) return;

    try {
      const doc = iframe.contentDocument || iframe.contentWindow.document;
      const newHeight = Math.max(
        doc.body.scrollHeight,
        doc.documentElement.scrollHeight,
        doc.body.offsetHeight,
        doc.documentElement.offsetHeight
      );
      iframe.style.height = newHeight + "px";
    } catch (e) {
      iframe.style.height = "calc(100vh - 140px)";
    }
  }

  window.addEventListener("load", resizeViewerFrame);
  window.addEventListener("resize", resizeViewerFrame);

  document.addEventListener("DOMContentLoaded", function () {
    const iframe = document.getElementById("viewer-frame");
    if (!iframe) return;

    iframe.addEventListener("load", function () {
      resizeViewerFrame();
      setTimeout(resizeViewerFrame, 200);
      setTimeout(resizeViewerFrame, 800);
    });
  });
</script>