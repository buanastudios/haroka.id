---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: biolink
---

<!-- <div class="swiper-slide swiper-slide-prev swiper-slide-duplicate-next" role="group" aria-roledescription="slide" aria-label="2 / 2" data-swiper-slide-index="1" style="width: 480px;" aria-hidden="true" inert=""><figure class="swiper-slide-inner"><img data-lazyloaded="1" src="https://larisko.com/wp-content/uploads/2025/02/WhatsApp-Image-2025-02-01-at-22.47.23.jpeg" decoding="async" class="swiper-slide-image entered litespeed-loaded" data-src="https://larisko.com/wp-content/uploads/2025/02/WhatsApp-Image-2025-02-01-at-22.47.23.jpeg" alt="WhatsApp Image 2025-02-01 at 22.47.23" data-ll-status="loaded"><noscript><img decoding="async" class="swiper-slide-image" src="https://larisko.com/wp-content/uploads/2025/02/WhatsApp-Image-2025-02-01-at-22.47.23.jpeg" alt="WhatsApp Image 2025-02-01 at 22.47.23" /></noscript></figure></div> -->

<style>
	.slider {
  width: 300px;
  text-align: center;
  overflow: hidden;
}

.slides {
  display: flex;
  
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  
  
  
  scroll-behavior: smooth;
  -webkit-overflow-scrolling: touch;
  
  /*
  scroll-snap-points-x: repeat(300px);
  scroll-snap-type: mandatory;
  */
}
.slides::-webkit-scrollbar {
  width: 10px;
  height: 10px;
}
.slides::-webkit-scrollbar-thumb {
  background: black;
  border-radius: 10px;
}
.slides::-webkit-scrollbar-track {
  background: transparent;
}
.slides > div {
  scroll-snap-align: start;
  flex-shrink: 0;
  width: 300px;
  height: 300px;
  margin-right: 50px;
  border-radius: 10px;
  background: #eee;
  transform-origin: center center;
  transform: scale(1);
  transition: transform 0.5s;
  position: relative;
  
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 100px;
}
.slides > div:target {
/*   transform: scale(0.8); */
}
.author-info {
  background: rgba(0, 0, 0, 0.75);
  color: white;
  padding: 0.75rem;
  text-align: center;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  margin: 0;
}
.author-info a {
  color: white;
}

.slider img {
  object-fit: cover;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.slider > a {
  display: inline-flex;
  width: 1.5rem;
  height: 1.5rem;
  background: white;
  text-decoration: none;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  margin: 0 0 0.5rem 0;
  position: relative;
}
.slider > a:active {
  top: 1px;
}
.slider > a:focus {
  background: #000;
}

/* Don't need button navigation */
@supports (scroll-snap-type) {
  .slider > a {
    display: none;
  }
}
</style>
<div class="slider">  
  <a href="#slide-1">1</a>
  <a href="#slide-2">2</a>
  <a href="#slide-3">3</a>
  <a href="#slide-4">4</a>
  <a href="#slide-5">5</a>

  <div class="slides">
    <div id="slide-1">
      1
    </div>
    <div id="slide-2">
      2
    </div>
    <div id="slide-3">
      3
    </div>
    <div id="slide-4">
      4
    </div>
    <div id="slide-5">
      5
    </div>
  </div>
</div>