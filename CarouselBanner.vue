<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="10000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="260"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=54">
        <h1>An Architectural Eye</h1>
        <h2>Come in and Explore</h2>
      </b-carousel-slide>

      <!-- slide with custom text #2 -->
      <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=58">
        <h1>An Architectural Eye</h1>
        <h2>Come in and Explore</h2>
      </b-carousel-slide>

      <!-- slide with custom text #3 -->
      <!-- <b-carousel-slide img-src="https://picsum.photos/1024/480/?image=55"> -->
      <b-carousel-slide img-src="~@/assets/tallBannerFirstCard.png">
        <h1>An Architectural Eye</h1>
        <h2>Come in and Explore</h2>
      </b-carousel-slide>

      <!-- Slide with blank fluid image to maintain slide aspect ratio -->
    </b-carousel>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>
