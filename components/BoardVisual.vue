<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="hello!"
        text="남건의 게시판에 방문해주셔서 감사합니다~!"
        :img-src="require('../static/vpic1.jpg')"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide :img-src="require('../static/vpic2.jpg')">
        <h1>Hello Nam Geon!</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide :img-src="require('../static/vpic3.jpg')"></b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide :img-src="require('../static/vpic4.jpg')">
      </b-carousel-slide>

     <b-carousel-slide :img-src="require('../static/vpic5.jpg')">
        <h1>Hello!</h1>
      </b-carousel-slide>
    </b-carousel>

    <p class="mt-4">
      Slide #: {{ slide }}<br>
      Sliding: {{ sliding }}
    </p>
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