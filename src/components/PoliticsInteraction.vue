<template>
  <div class="politics-interaction clearfix">
    <img src="../static/img/政民互动@3x.png" class="title-img" />
    <div class="left">
      <div class="head">
        <span class="title">最热诉求</span>
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
    <div class="center">
      <div class="head">
        <span class="title">最新诉求</span>
      </div>
      <ul class="title-content">
        <li v-for="index in 10" :key="index">
          <p>
            直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
          </p>
        </li>
      </ul>
    </div>
    <div class="right">
      <div class="head">
        <span class="title">诉求入口</span>
      </div>
      <div class="click bg1">投诉举报</div>
      <div class="click bg2">我要求助</div>
      <div class="click bg3">我要咨询</div>
      <div class="click bg4">我要建议</div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.politics-interaction {
  width: 100%;
  border: 1px solid #d9d9d9;
  border-top: none;
  margin-bottom: 30px;
  .title-img {
    width: 100%;
    margin-bottom: 10px;
  }
  .left {
    float: left;
    margin-left: 8px;
    width: 188px;
    height: 408px;
    border: 1px solid #d9d9d9;
    margin-bottom: 10px;
  }
  .center {
    float: left;
    margin-left: 20px;
    width: 494px;
    height: 408px;
    border: 1px solid #d9d9d9;
  }
  .right {
    float: left;
    margin-left: 20px;
    width: 262px;
    height: 408px;
    border: 1px solid #d9d9d9;
    img {
      width: 210px;
      height: 62px;
    }
    .click {
      width: 210px;
      height: 62px;
      color: white;
      font-size: 18px;
      text-align: center;
      line-height: 62px;
      margin: 20px auto 0;
    }
    .bg1 {
      background-image: url("../static/img/投诉举报.png");
      margin-top: 28px;
    }
    .bg2 {
      background-image: url("../static/img/我要求助.png");
    }
    .bg3 {
      background-image: url("../static/img/我要咨询.png");
    }
    .bg4 {
      background-image: url("../static/img/我要建议.png");
    }
  }
}
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
  width: 100%;
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
</style>
