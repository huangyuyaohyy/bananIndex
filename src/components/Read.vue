<template>
  <div class="read clearfix">
    <img src="../static/img/文学悦读@3x.png" class="title-img" />
    <div class="left">
      <div class="head">
        <span class="title">巴渝龙门阵</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <img
        src="http://imagecdn.cqliving.com/images/app_34/cms/202005/1e1a6c5f52c5458ab8dec738ba2df23d.jpg"
      />
      <ul class="title-content">
        <li v-for="index in 4" :key="index">
          <p>
            直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
          </p>
        </li>
      </ul>
    </div>
    <div class="center">
      <div class="head">
        <span class="title">悦读文摘</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <div class="img-content clearfix">
        <div class="l">
          <img
            src="http://imagecdn.cqliving.com/images/app_34/cms/201911/e8ffed57e61b4a44b19a562b47a98053.jpg"
          />
          <p>111111111111111111111111111111</p>
        </div>
        <div class="r">
          <img
            src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          />
          <p>11111111111</p>
        </div>
      </div>
      <ul class="title-content">
        <li v-for="index in 6" :key="index">
          <p>
            直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
          </p>
        </li>
      </ul>
    </div>
    <div class="right">
      <div class="head">
        <span class="title">全媒体</span>
      </div>
      <img src="../static/img/巴南微发布.png" class="banan-titile top" />
      <img src="../static/img/巴南日报微博.png" class="banan-titile" />
      <img src="../static/img/巴南日报数字报.png" class="banan-titile" />
      <img src="../static/img/巴南手机报.png" class="banan-titile" />
      <div class="weixin clearfix">
        <div class="l">
          <img
            src="http://imagecdn.cqliving.com/images/app_0/cms/201905/2fc5678ea8f04bab9f544b5f622a3d73.png"
          />
          <div class="text">关注看巴南公众号</div>
        </div>
        <div class="r">
          <img
            src="http://imagecdn.cqliving.com/images/app_0/cms/201905/5913a7eaff194c13a0ebd279e9bc9374.png"
          />
          <div class="text">下载看巴南APP</div>
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.read {
  width: 100%;
  margin-bottom: 20px;
  .title-img {
    width: 100%;
    margin-bottom: 10px;
  }
  .left {
    float: left;
    margin-left: 8px;
    width: 368px;
    height: 408px;
    border: 1px solid #d9d9d9;
    margin-bottom: 10px;
    img {
      width: 342px;
      height: 196px;
      margin-top: 10px;
      margin-left: 14px;
      border-radius: 3px;
    }
  }
  .center {
    float: left;
    margin-left: 10px;
    width: 336px;
    height: 408px;
    border: 1px solid #d9d9d9;
    .img-content {
      img {
        width: 150px;
        height: 100px;
        border-radius: 3px;
        // vertical-align: top; //取消img自带间隙
        margin-top: 10px;
        display: block;
      }
      p {
        width: 80%;
        color: #333;
        font-size: 14px;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
        line-height: 14px;
        margin-top: 8px;
        margin-bottom: 6px;
      }
      .l {
        margin-left: 10px;
        width: 150px;
        float: left;
      }
      .r {
        margin-left: 12px;
        width: 150px;
        float: left;
      }
    }
  }
  .right {
    float: left;
    margin-left: 10px;
    width: 260px;
    height: 408px;
    border: 1px solid #d9d9d9;
    .banan-titile {
      margin-left: 10px;
      margin-top: 12px;
      border-radius: 3px;
      // vertical-align: top; //取消img自带间隙
      margin-top: 10px;
      display: block;
    }
    .top {
      margin-top: 16px;
    }
    .weixin {
      text-align: center;
      img {
        margin-top: 6px;
        width: 94px;
        height: 94px;
      }
      .text {
        width: 104px;
        height: 28px;
        line-height: 28px;
        background-color: #ef7900;
        color: #fff;
        font-size: 12px;
      }
      .l {
        float: left;
        margin-left: 18px;
      }
      .r {
        float: left;
        margin-left: 18px;
      }
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
