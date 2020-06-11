<template>
  <div class="health clearfix">
    <img src="../static/img/健康养生@3x.png" class="title-img" />
    <div class="left"><swipe height="340px"></swipe></div>
    <div class="right">
      <ul class="title-content">
        <li v-for="index in 10" :key="index">
          <p>
            直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
import Swipe from "./Swipe.vue";
export default {
  components: { Swipe }
};
</script>
<style lang="scss" scoped>
.health {
  width: 100%;
  padding-bottom: 10px;
  border: 1px solid #d9d9d9;
  border-top: none;
  margin-bottom: 26px;
  .title-img {
    width: 100%;
    display: block;
  }
  .left {
    float: left;
    width: 620px;
    height: 340px;
    margin-top: 26px;
  }
  .right {
    float: left;
    margin-left: 22px;
  }
}
.title-content {
  width: 358px;
  margin-top: 22px;
  li {
    margin-top: 18px;
    line-height: 18px;
    padding-left: 32px;
    list-style-type: none;
    // 三角形图标
    background-image: url("../static/img/三角形.png");
    background-repeat: no-repeat;
    background-position: 16px center;
    p {
      width: 95%;
      color: #353535;
      font-size: 16px;
      text-decoration: none;
      overflow: hidden;
      text-overflow: ellipsis;
      cursor: pointer;
      white-space: nowrap;
    }
    p:hover {
      text-decoration: underline;
    }
  }
}
</style>
