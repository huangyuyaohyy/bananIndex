<template>
  <div class="tv-news">
    <img src="../static/img/电视新闻@3x.png" class="title-img" />
    <div class="click"></div>
    <div class="tv-player-div clearfix">
      <div class="left">
        <a href="javascript:;"
          ><img
            class="cover-img"
            src="http://imagecdn.cqliving.com/images/app_34/cms/202003/77ed71ab5bc94acb93f3a37c375a1dea.jpg"
          />
          <img class="player-icon" src="../static/img/播放按钮.png" />
          <p>巴南区市管理局选用科学举办保健食品xxxxxxxxxxxxxxxxxx</p>
        </a>
      </div>
      <div class="right">
        <a
          href="javascript:;"
          v-for="index in 6"
          :key="index"
          :class="{ leftzero: index % 3 == 1, top: index > 3 }"
          title="巴南区市管理局选用科学举办保健食品xxxxxxxxxxxxxxxaaaaaaaaabbbbb"
          ><img
            class="cover-img"
            src="http://imagecdn.cqliving.com/images/app_34/cms/202003/77ed71ab5bc94acb93f3a37c375a1dea.jpg"
          />
          <img class="player-icon" src="../static/img/播放按钮.png" />
          <p>巴南区市管理局选用科学举办保健食品xxxxxxxxxxxxxxxaaaaaaaaabbbbb</p>
        </a>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.tv-news {
  width: 100%;
  border: 1px solid #d9d9d9;
  border-top: none;
  margin-bottom: 28px;
  position: relative;
  .title-img {
    width: 100%;
    margin-bottom: 18px;
  }
  .click {
    width: 45px;
    height: 16px;
    position: absolute;
    right: 35px;
    top: 16px;
  }
  .click:hover {
    border-bottom: 1px solid #ef7900;
    cursor: pointer;
  }
  .tv-player-div {
    .left {
      width: 376px;
      height: 300px;
      border: 1px solid #d9d9d9;
      float: left;
      margin-left: 8px;
      margin-bottom: 20px;
      a {
        display: block;
        margin-top: 20px;
        margin-left: 10px;
        text-decoration: none;
        position: relative;
        .cover-img {
          width: 350px;
          height: 230px;
          vertical-align: top;
        }
        .player-icon {
          position: absolute;
          width: 54px;
          height: 54px;
          top: 90px;
          left: 150px;
        }
        p {
          margin-top: 14px;
          width: 95%;
          white-space: nowrap;
          overflow: hidden;
          text-overflow: ellipsis;
          font-size: 16px;
          line-height: 16px;
          color: #333;
        }
      }
    }
    .right {
      width: 588px;
      height: 300px;
      float: right;
      margin-right: 8px;
      .leftzero {
        margin-left: 0px;
      }
      .top {
        margin-top: 8px;
      }
      a {
        display: block;
        text-decoration: none;
        position: relative;
        float: left;
        width: 180px;
        margin-left: 24px;
        .cover-img {
          width: 180px;
          height: 110px;
          vertical-align: top;
        }
        .player-icon {
          position: absolute;
          width: 42px;
          height: 42px;
          top: 34px;
          left: 70px;
        }
        p {
          margin-top: 6px;
          // width: 100%;
          font-size: 12px;
          line-height: 16px;
          color: #333;
          width: 100%;
          // 两行文本省略
          // display: -webkit-box;
          // -webkit-box-orient: vertical;
          // -webkit-line-clamp: 2;
          // overflow: hidden;
          text-overflow: -o-ellipsis-lastline;
          overflow: hidden;
          text-overflow: ellipsis;
          display: -webkit-box;
          -webkit-line-clamp: 2;
          line-clamp: 2;
          -webkit-box-orient: vertical;
        }
      }
    }
  }
}
</style>
