<template>
  <div>
    <o-carousel :selected.sync="select" autoplay>  
      <carousel-item name="1">
        <div class="box">1</div>
      </carousel-item>
      <carousel-item name="2">
        <div class="box">2</div>
      </carousel-item>
      <carousel-item name="3">
        <div class="box">3</div>
      </carousel-item>
      <carousel-item name="4">
        <div class="box">4</div>
      </carousel-item>
    </o-carousel>
    <pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import Carousel from '../../../src/components/carousel/carousel'
import CarouselItem from '../../../src/components/carousel/carousel-item'
export default {
  components: {
    'o-carousel': Carousel,
    'carousel-item': CarouselItem
  },
  data() {
    return {
      select: '',
      content: `
<o-carousel :selected.sync="select" autoplay>  
  <carousel-item name="1">
    <div class="box">1</div>
  </carousel-item>
  <carousel-item name="2">
    <div class="box">2</div>
  </carousel-item>
  <carousel-item name="3">
    <div class="box">3</div>
  </carousel-item>
  <carousel-item name="4">
    <div class="box">4</div>
  </carousel-item>
</o-carousel>

data() {
  retrun {select: ''}
}      
`.trim()
    }
  }
}
</script>
<style lang="scss" scoped>
.box {
      height: 300px;
      width: 700px;
      background-color: #46a1de;
      display: inline-flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      font-size: 32px;
    }
</style>

