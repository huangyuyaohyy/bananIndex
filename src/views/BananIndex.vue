<template>
  <div class="banan-index">
    <el-backtop :right="80" :bottom="50">
      <img src="../static/img/滑至顶部@3x.png" style="width:40px;height:40px" />
    </el-backtop>
    <div class="bg">
      <img src="../assets/bg.png" width="100%" alt="bg" />
    </div>
    <div class="content">
      <span class="close-bg" @click="closeBg">关闭</span>
      <header class="header">
        <img src="../static/img/logo.png" alt="title" class="title-logo" />
        <div class="search-div">
          <div class="search">
            <img src="../static/img/搜索.png" class="search-icon" />
            <input
              type="text"
              class="search-input"
              placeholder="请输入搜索关键词进行搜索"
            />
          </div>
        </div>
      </header>
      <nav>
        <ul class="nav">
          <li class="index"><a href="javascript:;">首页</a></li>
          <li class="news-item">
            <a class="a">头条新闻</a>
            <ul class="drop-item news-drop">
              <li><a>头条</a></li>
              <li><a>原创热点</a></li>
              <li><a>巴南热点</a></li>
            </ul>
          </li>
          <li><a href="javascript:;">电视新闻</a></li>
          <li class="public-item">
            <a class="a" href="javascript:;">政务公开</a>
            <ul class="drop-item public-drop">
              <li><a>通知公告</a></li>
              <li><a>最新政策</a></li>
              <li><a>信息发布</a></li>
            </ul>
          </li>

          <li><a href="javascript:;">政民互动</a></li>
          <li><a href="javascript:;">文学悦读</a></li>
          <li class="travel-item">
            <a class="a" href="javascript:;">休闲旅游</a>
            <ul class="drop-item travel-drop">
              <li><a>吃巴南</a></li>
              <li><a>游巴南</a></li>
              <li><a>行巴南</a></li>
              <li><a>购巴南</a></li>
              <li><a>住巴南</a></li>
            </ul>
          </li>

          <li class="live-item">
            <a class="a" href="javascript:;">便民生活</a>
            <ul class="drop-item live-drop">
              <li><a>美食</a></li>
              <li><a>房市</a></li>
              <li><a>车市</a></li>
            </ul>
          </li>

          <li><a href="javascript:;">健康养生</a></li>
          <li><a href="javascript:;">精彩图库</a></li>
        </ul>
      </nav>
      <section>
        <div class="news-title-swipe">
          <img src="../static/img/新闻推荐.png" class="news-title-img" />
          <TextSwipe class="swiper" :text="newsTitleSwipe"></TextSwipe>
        </div>
        <Headline></Headline>
        <SwipeContent></SwipeContent>
        <TvNews></TvNews>
        <img src="../static/img/banner.png" class="banner" />
        <div class="politics-daily clearfix">
          <div class="politics">
            <PoliticsPublishment></PoliticsPublishment>
          </div>
          <div class="daily"><BananDaily></BananDaily></div>
        </div>
        <PoliticsInteraction></PoliticsInteraction>
        <img src="../static/img/banner.png" class="banner" />
        <Read></Read>
        <travel></travel>
        <img
          src="../static/img/banner.png"
          class="banner"
          style="margin-bottom:10px;"
        />
        <Health></Health>
        <pictures></pictures>
      </section>
    </div>
    <BananFooter></BananFooter>
  </div>
</template>
<script>
import TextSwipe from "../components/TextSwipe.vue";
import Headline from "../components/Headline.vue";
import TvNews from "../components/TvNews.vue";
import PoliticsPublishment from "../components/PoliticsPublishment.vue";
import BananDaily from "../components/BananDaily.vue";
import PoliticsInteraction from "../components/PoliticsInteraction.vue";
import Read from "../components/Read.vue";
import Travel from "../components/Travel.vue";
import Health from "../components/Health.vue";
import Pictures from "../components/Pictures.vue";
import BananFooter from "../components/BananFooter.vue";
import SwipeContent from "../components/SwipeContent.vue";
import { Backtop, PageHeader } from "element-ui";
export default {
  data() {
    return {
      newsTitleSwipe: [
        "你最帅！穿梭在李家沱社区的“红马甲”媒体人",
        "守望相助，爱不止步！",
        "一品街道商会捐赠疫情防控物资暖民心",
        "安澜有支人居环境志愿服务队，主动请缨为居民清扫环境"
      ]
    };
  },
  components: {
    TextSwipe,
    Headline,
    TvNews,
    PoliticsPublishment,
    BananDaily,
    PoliticsInteraction,
    Read,
    Travel,
    Health,
    Pictures,
    BananFooter,
    SwipeContent,
    [Backtop.name]: Backtop,
    [PageHeader.name]: PageHeader
  },
  methods: {
    closeBg() {
      const close = document.querySelector(".close-bg");
      const bgImg = document.querySelector(".bg");
      const content = document.querySelector(".content");
      bgImg.style.display = "none";
      close.style.display = "none";
      content.style.margin = "0 auto";
    }
  }
};
</script>
<style lang="scss" scoped>
.bg {
  position: absolute;
  top: 0;
  z-index: -1;
}
.content {
  position: relative;
  width: 1000px;
  margin: 220px auto 0px;
  background-color: white;
  z-index: 1;
  // 媒体查询
  // @media screen and (min-width: 1366px) {
  //   width: 1200px;
  // }
  .close-bg {
    font-size: 24px;
    color: #333333;
    font-family: "Microsoft YaHei[Regular]";
    position: absolute;
    right: 0;
    top: -46px;
    cursor: pointer;
    cursor: hand; //ie5
    line-height: 1;
  }
  header {
    width: 100%;
    height: 70px;
    position: relative;
    .title-logo {
      width: 164px;
      height: 52px;
      position: absolute;
      top: 50%; //50%并不是居中的，因为它是以元素的上border为标准移动50%的
      transform: translateY(
        -50%
      ); //所以我们需要像上移动元素自身高度一半儿的距离
      left: 8px;
    }
    .search-div {
      width: 226px;
      height: 28px;
      border: 1px solid #cccccc;
      border-radius: 5px;
      position: absolute;
      top: 50%; //50%并不是居中的，因为它是以元素的上border为标准移动50%的
      transform: translateY(
        -50%
      ); //所以我们需要像上移动元素自身高度一半儿的距离
      right: 42px;
      overflow: hidden;
      .search {
        white-space: nowrap; //不允许换行
        position: relative;
        height: 28px;
        .search-icon {
          position: absolute;
          width: 16px;
          height: 18px;
          left: 22px;
          top: 5px;
        }
        .search-input {
          margin-left: 16px;
          width: 170px;
          height: 24px;
          font-size: 12px;
          position: absolute;
          right: 0;
          border: 0; //去边框
          outline: medium; //聚焦时也无边框
          top: 50%; //50%并不是居中的，因为它是以元素的上border为标准移动50%的
          transform: translateY(-50%);
        }
      }
    }
  }
  nav {
    width: 100%;
    height: 38px;
    background-color: #ef7900;
    border-radius: 3px;
    .nav {
      height: 38px;
      line-height: 38px;
      text-align: center;
      .index {
        font-weight: 700;
      }
      li {
        list-style-type: none;
        display: inline-table;
        width: 98px;
        height: 38px;
        text-align: center;
        a {
          text-decoration: none;
          color: #ffffff;
          font-size: 16px;
        }
        a:hover {
          font-weight: 700;
          border-bottom: 2px solid #ffffff;
        }
        .drop-item {
          display: none;
          width: 98px;
          background-color: #ef7900;
          padding: 20px 0;
          position: relative;
          z-index: 999;
          li {
            list-style-type: none;
          }
        }
      }
      // 经过某个导航栏，相应的二级目录显示
      .news-item:hover .a {
        border-bottom: 0;
      }
      .news-item:hover .news-drop {
        display: block;
      }
      .public-item:hover .a {
        border-bottom: 0;
      }
      .public-item:hover .public-drop {
        display: block;
      }
      .travel-item:hover .a {
        border-bottom: 0;
      }
      .travel-item:hover .travel-drop {
        display: block;
      }
      .live-item:hover .a {
        border-bottom: 0;
      }
      .live-item:hover .live-drop {
        display: block;
      }
    }
  }
  .news-title-swipe {
    width: 100%;
    height: 46px;
    background-color: #fbf1f2;
    position: relative;
    z-index: -1;
    .news-title-img {
      width: 84px;
      height: 34px;
      position: absolute;
      top: 50%; //50%并不是居中的，因为它是以元素的上border为标准移动50%的
      transform: translateY(-50%);
      left: 20px;
    }
    .swiper {
      width: 860px;
      margin-left: 138px;
    }
  }
  .banner {
    width: 100%;
    height: 110px;
    margin-bottom: 28px;
  }
  .politics-daily {
    .politics {
      float: left;
    }
    .daily {
      float: right;
    }
  }
}
</style>
