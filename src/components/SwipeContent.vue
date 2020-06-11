<template>
  <div class="swipe-content">
    <!-- <a
      class="swiper-item"
      href="javascript:;"
      title="大视野看巴南啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦"
      v-for="item in 6"
      :key="item"
    >
      <img
        src="http://imagecdn.cqliving.com/images/app_34/cms/202003/bbf57481c400440eaf98656cfc0b81f1.jpg"
      />
      <p class="swiper-title">大视野看巴南啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦</p>
      <p class="swiper-sub-title">
        大视野看巴南啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦
      </p>
    </a> -->
    <div class="left-icon" slot="button-prev">
      <img class="next-icon" src="../static/img/下一步.png" />
    </div>
    <div class="right-icon" slot="button-next">
      <img
        class="next-icon"
        src="../static/img/下一步.png"
        style="transform:rotate(180deg)"
      />
    </div>
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide v-for="item in 9" :key="item" class="swiper-slide-item"
        ><a
          class="swiper-item"
          href="javascript:;"
          title="大视野看巴南啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦"
        >
          <img
            src="http://imagecdn.cqliving.com/images/app_34/cms/202003/bbf57481c400440eaf98656cfc0b81f1.jpg"
          />
          <p class="swiper-title">
            大视野看巴南啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦
          </p>
          <p class="swiper-sub-title">
            大视野看巴南啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦啦
          </p>
          <img src="../static/img/【进入】.png" class="inter" />
        </a>
      </swiper-slide>

      <!-- <div class="swiper-pagination" slot="pagination"></div> -->
    </swiper>
  </div>
</template>
<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";
export default {
  name: "swiper-example-loop-group",
  title: "Loop mode with multiple slides per group",
  components: {
    Swiper,
    SwiperSlide
  },
  data() {
    return {
      swiperOption: {
        slidesPerView: "auto",
        spaceBetween: 20,
        slidesPerGroup: 3,
        // loop: true,
        // autoplay: true,
        // 自动播放
        autoplay: {
          delay: 1500,
          stopOnLastSlide: false,
          disableOnInteraction: false
        },
        loopFillGroupWithBlank: true,
        pagination: {
          el: ".swiper-pagination",
          clickable: true
        },
        navigation: {
          nextEl: ".left-icon",
          prevEl: ".right-icon"
        }
      }
    };
  }
};
</script>
<style lang="scss" scoped>
.swipe-content {
  margin-top: 40px;
  margin-bottom: 30px;
  border: 1px solid #d9d9d9;
  width: 100%;
  height: 286px;
  position: relative;
  .next-icon {
    width: 36px;
    height: 36px;
  }
  .left-icon {
    position: absolute;
    left: 12px;
    top: 90px;
    width: 36px;
  }
  .right-icon {
    position: absolute;
    right: 12px;
    top: 90px;
    width: 36px;
  }
  .swiper {
    width: 860px;
    .swiper-slide-item {
      width: 200px !important;
      // margin-right: 0px !important;
      // margin-left: 20px;
      margin-top: 16px;
    }
  }
  .swiper-item {
    display: block;
    width: 200px;
    position: relative;
    img {
      width: 200px;
      height: 154px;
      border-radius: 3px;
    }
    .swiper-title {
      margin-top: 20px;
      font-size: 20px;
      line-height: 20px;
      color: #222;
      //单行文本省略
      width: 100%;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
    }
    .swiper-sub-title {
      margin-top: 10px;
      font-size: 14px;
      color: #666;
      line-height: 20px;
      //双行文本省略
      display: -webkit-box;
      -webkit-box-orient: vertical;
      -webkit-line-clamp: 2;
      overflow: hidden;
    }
    .inter {
      width: 48px;
      height: 16px;
      position: absolute;
      right: 0;
      bottom: 0;
    }
  }
}
</style>

<style>
.swiper-button-next:after,
.swiper-container-rtl .swiper-button-prev:after {
  content: "";
}
.swiper-button-prev:after,
.swiper-container-rtl .swiper-button-next:after {
  content: "";
}

:focus {
  outline: none;
}
</style>
