<template>
  <b-carousel
  id="carousel-fade"
  style="text-shadow: 0px 0px 2px #000"
  fade
  :interval="0"
  indicators
  controls
  img-width="1024"
  img-height="480"
>
  <b-carousel-slide caption="First slide" text="Nulla vitae elit libero, a pharetra augue mollis interdum." img-src="https://picsum.photos/1024/480/?image=10"></b-carousel-slide>
  <b-carousel-slide caption="Second Slide" text="Nulla vitae elit libero, a pharetra augue mollis interdum." img-src="https://picsum.photos/1024/480/?image=12"></b-carousel-slide>
  <b-carousel-slide caption="Third Slide" text="Nulla vitae elit libero, a pharetra augue mollis interdum." img-src="https://picsum.photos/1024/480/?image=22"></b-carousel-slide>
</b-carousel>
</template>
