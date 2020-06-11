<template>
  <div class="hot-point">
    <div class="head">
      <span class="title">{{ title }}</span>
      <a href="javascript:;" class="more">更多》</a>
    </div>
    <ul class="title-content">
      <li v-for="index in 10" :key="index">
        <p>
          直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
        </p>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  props: {
    title: {
      type: String
    }
  }
};
</script>
<style lang="scss" scoped>
.hot-point {
  width: 482px;
  height: 408px;
  border: 1px solid #d9d9d9;
  .head {
    width: 100%;
    height: 40px;
    line-height: 40px;
    background-color: #fbf1f2;
    span {
      color: #c43a4a;
      font-size: 16px;
      float: left;
      margin-left: 16px;
      font-weight: 700;
    }
    .more {
      float: right;
      color: #666666;
      font-size: 14px;
      text-decoration: none;
      margin-right: 22px;
    }
    .more:hover {
      text-decoration: underline;
    }
  }
  .title-content {
    width: 420px;
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
        width: 90%;
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
}
</style>
