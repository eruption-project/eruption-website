+++
title = "Screenshots and Videos"
path = "gallery"
slug = "gallery"
paginate_by = 5
weight = 10
author = "X3n0m0rph59"
date = 2022-05-11
+++

<div class="pswp-gallery pswp-gallery--single-column" id="my-gallery">
  <h4>Eruption GUI</h4>

  <a href="/img/screenshot-01.png"
    data-pswp-width="1492"
    data-pswp-height="881"
    target="_blank">
    <img src="/img/screenshot-01.png" alt="Eruption GUI - Keyboard devices" />
  </a>
  <a href="/img/screenshot-02.png"
    data-pswp-width="1492"
    data-pswp-height="881"
    target="_blank">
    <img src="/img/screenshot-02.png" alt="Eruption GUI - Mouse devices" />
  </a>
 <a href="/img/screenshot-03.png"
    data-pswp-width="1492"
    data-pswp-height="881"
    target="_blank">
    <img src="/img/screenshot-03.png" alt="Eruption GUI - Process Monitor" />
  </a>

  <h4>Profile Switcher Extension</h4>

  <a href="/img/screenshot-profile-switcher-01.jpg"
    data-pswp-width="353"
    data-pswp-height="546"
    target="_blank">
    <img src="/img/screenshot-profile-switcher-01.jpg" alt="Profile Switcher" />
  </a>
  <a href="/img/screenshot-profile-switcher-02.jpg"
    data-pswp-width="435"
    data-pswp-height="1080"
    target="_blank">
    <img src="/img/screenshot-profile-switcher-02.jpg" alt="Profile Switcher" />
  </a>
  </div>
</div>

<div class="spacer-xs"></div>

#### Videos on YouTube

[![Eruption Video](https://img.youtube.com/vi/ig_71zg14nQ/0.jpg)](https://www.youtube.com/watch?v=ig_71zg14nQ)


<script type="module">
import Lightbox from '/js/photoswipe/photoswipe-lightbox.esm.min.js';
const lightbox = new Lightbox({
  gallery: '#my-gallery',
  children: 'a',
  pswpModule: () => import('/js/photoswipe/photoswipe.esm.min.js')
});
lightbox.init();
</script>

<link rel="stylesheet" href="/css/photoswipe.css">
