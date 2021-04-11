<template>
  <div id="head">
    <div id="head-content">
      <div id="favicon">
        <img src="~assets/img/logo.png" alt="" />
      </div>
      <div id="title">异空间</div>
      <div id="download">
        <a
          href="http://oss.tuzidewang.xyz//apks/154544c9a29e4f7f81bfa5f999ee6690.apk"
        >
          <!-- <img src="~assets/img/android.png" alt="" /> -->
          下载APP
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "head",
  mounted: function () {
    window.addEventListener("scroll", this.handleScroll, false); // 监听（绑定）滚轮滚动事件
  },

  methods: {
    handleScroll: function () {
      let scrollObj = document.getElementById("head"); // 滚动区域
      let ObjTop = scrollObj.offsetTop; // div 到头部的距离
      let ObjHeight = scrollObj.offsetHeight;
      if (window.pageYOffset >= ObjTop + ObjHeight) {
        scrollObj.style.position = "fixed";
        scrollObj.top = 0 + "px";
      } else {
        scrollObj.style.position = "relative";
      }
    },
  },

  destroyed: function () {
    window.removeEventListener("scroll", this.handleScroll); //  离开页面清除（移除）滚轮滚动事件
  },
};
</script>

<style lang='less'>
#head {
  width: 100%;
  height: 49px;
  position: relative;
  top: 0;
  background-color: #fff;
  z-index: 100;
}
#head-content {
  height: 49px;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  padding-left: 10%;
  #favicon {
    img {
      width: 128/4px;
    }
  }
  #title {
    padding-left: 5px;
    color: #555;
    font-size: 20px;
  }
  #download {
    padding-left: 50%;
    a {
      display: inline-block;
      height: 30px;
      line-height: 30px;
      color: #551a8b;
      border: 1px solid #551a8b;
      border-radius: 5px;
    }
  }
}
</style>