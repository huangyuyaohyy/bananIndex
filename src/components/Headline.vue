<template>
  <div class="headline">
    <img src="../static/img/头条新闻@3x.png" class="title-img" />
    <div class="head-info clearfix">
      <div class="swipe-div">
        <Swipe height="406px"></Swipe>
      </div>
      <div class="head-title">
        <img class="head-title-img" src="../static/img/头条@3x.png" />
        <a class="more" href="javascript:;">更多》</a>
        <ul class="title-content">
          <li v-for="index in 10" :key="index">
            <p>
              11111111111111111111111111111111111111111111111111111111111111111111111
            </p>
          </li>
        </ul>
      </div>
    </div>
    <div class="hot-point-div clearfix">
      <div class="left"><HotPoint title="原创热点"></HotPoint></div>
      <div class="right"><HotPoint title="巴南热点"></HotPoint></div>
    </div>
  </div>
</template>
<script>
import Swipe from "./Swipe.vue";
import HotPoint from "./HotPoint.vue";
export default {
  components: {
    Swipe,
    HotPoint
  }
};
</script>
<style lang="scss" scoped>
.headline {
  border: 1px solid #d9d9d9;
  .title-img {
    width: 100%;
    margin-top: 30px;
    margin-bottom: 30px;
  }
  .head-info {
    position: relative;
    .swipe-div {
      width: 518px;
      height: 406px;
      float: left;
    }
    .head-title {
      height: 406px;
      float: right;
      margin-right: 15px;
      .head-title-img {
        width: 456px;
        height: 48px;
        vertical-align: top; //消除img自带间隙
      }
      .more {
        position: absolute;
        right: 15px;
        top: 10px;
        color: #ef7900;
        font-size: 16px;
        text-decoration: none;
      }
      .more:hover {
        text-decoration: underline;
      }
      .title-content {
        width: 420px;
        margin-top: 22px;
        li {
          margin-top: 18px;
          line-height: 18px;
          padding-left: 42px;
          list-style-type: none;
          // 三角形图标
          background-image: url("../static/img/三角形.png");
          background-repeat: no-repeat;
          background-position: 26px center;
          p {
            width: 92%;
            color: #353535;
            font-size: 16px;
            text-decoration: none;
            overflow: hidden;
            text-overflow: ellipsis;
            cursor: pointer;
          }
          p:hover {
            text-decoration: underline;
          }
        }
      }
    }
  }
  .hot-point-div {
    margin-top: 20px;
    margin-bottom: 30px;
    .left {
      float: left;
      margin-left: 8px;
    }
    .right {
      float: right;
      margin-right: 8px;
    }
  }
}
</style>
