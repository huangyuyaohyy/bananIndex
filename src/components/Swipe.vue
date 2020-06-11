<template>
  <div class="swipe">
    <el-carousel class="carousel" :height="height">
      <el-carousel-item v-for="item in imgs" :key="item">
        <img :src="item" :height="height" />
        <div class="mask">我是新闻标题~~</div>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>
<script>
import { Carousel, CarouselItem } from "element-ui";
export default {
  props: {
    height: {
      type: String
    }
  },
  data() {
    return {
      imgs: [
        "https://tse3-mm.cn.bing.net/th/id/OIP.9w3AK-_CaiWahcmVb7goOAHaEm?w=279&h=173&c=7&o=5&dpr=1.25&pid=1.7",
        "https://tse1-mm.cn.bing.net/th/id/OIP.rRtwquPCLO-KAD2EFJTb6AHaEr?w=300&h=189&c=7&o=5&dpr=1.25&pid=1.7",
        "http://i3.sinaimg.cn/dy/c/2014-02-13/U2004P1T1D29450305F21DT20140213080345.jpg"
      ]
    };
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
  // height: 406px;
  position: relative;
  img {
    width: 100%;
    // height: 406px;
  }
  .mask {
    width: 100%;
    height: 54px;
    line-height: 54px;
    position: absolute;
    bottom: 0;
    background-color: #000000;
    opacity: 28%;
    color: #ffffff;
    font-size: 20px;
  }
}
</style>
<style>
.el-carousel__indicators--horizontal {
  left: unset;
  right: 6px;
  transform: none;
}
.el-carousel__indicator--horizontal {
  padding: 2px 4px;
}
.el-carousel__button {
  width: 8px;
  height: 8px;
  border-radius: 50%;
}
</style>
