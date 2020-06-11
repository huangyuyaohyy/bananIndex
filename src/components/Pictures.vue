<template>
  <div class="pictures clearfix">
    <img src="../static/img/精彩图库@3x.png" class="title-img" />
    <div class="left clearfix">
      <div class="head">
        <span class="title">摄影沙龙</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
    </div>
    <div class="center clearfix">
      <div class="head">
        <span class="title">最美巴南</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
    </div>
    <div class="right clearfix">
      <div class="head">
        <span class="title">精彩瞬间</span>
        <a href="javascript:;" class="more">更多》</a>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
      <div class="img-text">
        <img
          src="http://imagecdn.cqliving.com/images/app_34/cms/201911/fde30988cf504a83992679f3b08a2d7a.jpg"
          class="content-img"
        />
        <p>养生泡汤团</p>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.pictures {
  width: 100%;
  padding-bottom: 20px;
  border: 1px solid #d9d9d9;
  border-top: none;
  padding-bottom: 16px;
  > div {
    float: left;
    margin-left: 20px;
    border: 1px solid #d9d9d9;
    height: 428px;
  }
  .title-img {
    width: 100%;
    display: block;
    margin-bottom: 10px;
  }
  .left {
    width: 236px;
    margin-left: 8px;
  }
  .center {
    width: 460px;
    .img-text {
      p {
        font-weight: 700;
        color: #353535;
      }
    }
  }
  .right {
    width: 248px;
  }
  .img-text {
    float: left;
    margin-top: 16px;
    .content-img {
      width: 212px;
      height: 140px;
      margin-left: 10px;
      display: block;
    }
    p {
      margin-top: 14px;
      margin-left: 10px;
      color: #333;
      font-size: 16px;
      line-height: 16px;
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
}
</style>
