<template>
  <div class="politics-publishment clearfix">
    <img src="../static/img/政务公开@3x.png" class="title-img" />
    <div class="left">
      <div class="head">
        <span class="title">通知公告</span>
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
    <div class="right">
      <div class="head">
        <span class="politics-title">信息发布</span>
        <span class="politics-title unfocus">最新政策</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <ul class="title-content politics-title-content">
        <li v-for="index in 10" :key="index">
          <p>
            直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
          </p>
        </li>
      </ul>
      <ul class="title-content politics-title-content nodispaly">
        <li v-for="index in 10" :key="index">
          <p>
            11111111111111111111111111111111111111111
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    const tab = document.querySelectorAll(".politics-title");
    const content = document.querySelectorAll(".politics-title-content");
    for (let i = 0; i < tab.length; i++) {
      tab[i].onclick = function() {
        for (let i = 0; i < tab.length; i++) {
          tab[i].className = "politics-title unfocus";
        }
        tab[i].className = "politics-title";
        for (let i = 0; i < content.length; i++) {
          content[i].style.display = "none";
        }
        content[i].style.display = "block";
      };
    }
  }
};
</script>
<style lang="scss" scoped>
.politics-publishment {
  width: 642px;
  height: 472px;
  border: 1px solid #d9d9d9;
  border-top: none;
  padding-bottom: 8px;
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
  }
  .right {
    float: left;
    margin-left: 20px;
    width: 418px;
    height: 408px;
    border: 1px solid #d9d9d9;
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
  .unfocus {
    color: #333;
    font-weight: 200;
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
.nodispaly {
  display: none;
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
