<template>
  <div class="banan-daily clearfix">
    <img src="../static/img/巴南日报@3x.png" class="title-img" />
    <img
      class="daily-img"
      src="http://nimage.cqliving.com/images/app_34/cms/2019-04-26/20194239517728.jpg"
    />
    <img src="../static/img/巴南手机报1.png" class="iphone-img" />
  </div>
</template>
<style lang="scss" scoped>
.banan-daily {
  width: 348px;
  height: 472px;
  border: 1px solid #d9d9d9;
  border-top: none;
  padding-bottom: 8px;
  .title-img {
    width: 100%;
  }
  .daily-img {
    width: 270px;
    height: 420px;
    margin-top: 4px;
    margin-left: 10px;
    float: left;
  }
  .iphone-img {
    float: left;
    margin-left: 20px;
    margin-top: 140px;
    cursor: pointer;
  }
}
</style>
