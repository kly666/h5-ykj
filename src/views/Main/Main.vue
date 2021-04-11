<template>
  <div id="main">
    <div id="wenan">
      <h3>异空间</h3>
      <p>隐藏各种格式文件数据</p>
      <p>守护你的手机秘密</p>
      <p>让隐私数据更安全</p>
    </div>
    <div id="main-img">
      <img src="~assets/img/main-img/main_img1.png" alt="" />
      <img src="~assets/img/main-img/main_img2.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style lang="less">
#main {
  padding-top: 20px;
  text-align: center;
  background-image: linear-gradient(90deg, #8a6441, #c2bb9b, #b29f94);

  #wenan {
    font-size: 20px;
    color: #fff;
    h3 {
      margin: 0;
      font-size: 28px;
    }
  }
  #main-img {
    position: relative;
    img {
      width: 60%;
    }
    img:first-child {
      margin-right: 100px;
    }
    img:last-child {
      top: 0;
      right: 17px;
      position: absolute;
    }
  }
}
</style>