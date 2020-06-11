<template>
  <div class="travel clearfix">
    <img src="../static/img/休闲旅游@3x.png" class="title-img" />
    <div class="left">
      <div class="head">
        <span class="title">吃在巴南</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <img
        src="http://imagecdn.cqliving.com/images/app_34/cms/202003/bda07a21f6a84ee38b07802404c78eac.jpg"
      />
      <span class="text-title">万州烤鱼（巴南店）</span>
      <ul class="title-content">
        <li v-for="index in 11" :key="index" :class="{ zore: index == 1 }">
          <p>
            直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
          </p>
        </li>
      </ul>
    </div>
    <div class="center">
      <div class="top clearfix">
        <div class="head">
          <span class="title">游在巴南</span>
          <a href="javascript:;" class="more">更多》</a>
        </div>
        <div class="content-left">
          <img
            src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          />
          <p class="text-title">东温泉景区</p>
          <ul class="title-content">
            <li v-for="index in 2" :key="index" class="center-li">
              <p>
                直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
              </p>
            </li>
          </ul>
        </div>
        <div class="content-right">
          <img
            src="http://imagecdn.cqliving.com/images/app_34/cms/201911/e8ffed57e61b4a44b19a562b47a98053.jpg"
          />
          <p class="text-title">巴南旅游</p>
          <ul class="title-content">
            <li v-for="index in 2" :key="index" class="center-li">
              <p>
                直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
              </p>
            </li>
          </ul>
        </div>
      </div>
      <div class="bottom clearfix">
        <div class="head">
          <span class="title">行在巴南</span>
          <a href="javascript:;" class="more">更多》</a>
        </div>
        <div class="content-left">
          <img
            src="http://imagecdn.cqliving.com/images/app_34/cms/202003/bda07a21f6a84ee38b07802404c78eac.jpg"
          />
          <p class="text-title">巴南年味浓</p>
        </div>
        <div class="content-right">
          <ul class="title-content">
            <li v-for="index in 6" :key="index" class="center-li">
              <p>
                直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
              </p>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="right">
      <div class="top">
        <div class="head">
          <span class="title">购在巴南</span>
          <a href="javascript:;" class="more">更多》</a>
        </div>
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/202003/bda07a21f6a84ee38b07802404c78eac.jpg"
        />
        <p class="text-title">巴南年味浓</p>
        <ul class="title-content">
          <li v-for="index in 3" :key="index" class="center-li">
            <p>
              直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
            </p>
          </li>
        </ul>
      </div>
      <div class="bottom">
        <div class="head">
          <span class="title">住在巴南</span>
          <a href="javascript:;" class="more">更多》</a>
        </div>
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/202003/bda07a21f6a84ee38b07802404c78eac.jpg"
        />
        <p class="text-title">巴南年味浓</p>

        <ul class="title-content">
          <li v-for="index in 3" :key="index" class="center-li">
            <p>
              直播回顾 | 巴南最大主播带货活动来啦，带你打卡三大网红商圈！
            </p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.travel {
  width: 100%;
  border: 1px solid #d9d9d9;
  border-top: none;
  margin-bottom: 24px;
  .title-img {
    width: 100%;
    margin-bottom: 10px;
  }
  .left {
    float: left;
    width: 252px;
    height: 522px;
    border: 1px solid #d9d9d9;
    margin-left: 8px;
    margin-bottom: 8px;
    img {
      width: 226px;
      height: 80px;
      display: block;
      margin-left: 12px;
      margin-top: 16px;
      margin-bottom: 12px;
    }
    .text-title {
      font-size: 16px;
      line-height: 16px;
      color: #333;
      font-weight: 700;
      margin-left: 16px;
    }
    .zore {
      margin-top: 14px;
    }
  }
  .center {
    float: left;
    width: 480px;
    height: 522px;
    margin-left: 12px;
    .top {
      img {
        width: 220px;
        height: 74px;
        border-radius: 3px;
        display: block;
        margin-top: 16px;
      }
      .text-title {
        font-size: 16px;
        line-height: 16px;
        color: #333;
        font-weight: 700;
        margin-top: 12px;
        margin-bottom: 20px;
      }
      .content-left {
        width: 220px;
        float: left;
        margin-left: 10px;
      }
      .content-right {
        width: 220px;
        float: left;
        margin-left: 16px;
      }
    }
    .bottom {
      .content-left {
        float: left;
        width: 45%;
        img {
          width: 180px;
          height: 150px;
          border-radius: 3px;
          margin-left: 10px;
          margin-top: 16px;
          margin-bottom: 13px;
        }
        .text-title {
          font-size: 16px;
          line-height: 16px;
          color: #353535;
          font-weight: 700;
          margin-left: 10px;
        }
      }
      .content-right {
        float: left;
        width: 55%;
      }
    }
    .center-li {
      line-height: 14px;
      padding-left: 16px;
      background-position: 0px center;
      color: #353535;
    }
  }
  .right {
    float: left;
    width: 228px;
    height: 522px;
    margin-left: 12px;
    img {
      width: 208px;
      height: 66px;
      margin-left: 10px;
      margin-top: 16px;
    }
    .center-li {
      line-height: 14px;
      padding-left: 26px;
      background-position: 10px center;
      color: #353535;
      p {
        font-size: 12px;
        line-height: 12px;
      }
    }
    .text-title {
      font-size: 14px;
      line-height: 14px;
      color: #353535;
      font-weight: 700;
      margin-left: 10px;
      margin-top: 10px;
    }
  }
  .top {
    width: 100%;
    height: 246px;
    border: 1px solid #d9d9d9;
  }
  .bottom {
    width: 100%;
    height: 258px;
    border: 1px solid #d9d9d9;
    margin-top: 20px;
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
  li {
    margin-top: 16px;
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
      font-size: 14px;
      line-height: 15px;
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
