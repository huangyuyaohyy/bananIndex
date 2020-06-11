<template>
  <div class="text-swipe">
    <el-carousel
      class="carousel"
      direction="vertical"
      indicator-position="none"
      height="46px"
    >
      <el-carousel-item class="carousel__item" v-for="item in text" :key="item">
        <a href="javascript:;">{{ item }}</a>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>
<script>
import { Carousel, CarouselItem } from "element-ui";
export default {
  data() {
    return {};
  },
  props: {
    text: {
      type: Array,
      required: true
    }
  },
  components: {
    [Carousel.name]: Carousel,
    [CarouselItem.name]: CarouselItem
  }
};
</script>
<style lang="scss" scoped>
.carousel {
  width: 100%;
}
.carousel__item a {
  color: #c43a4a;
  font-size: 16px;
  line-height: 46px;
  text-decoration: none;
}
</style>
