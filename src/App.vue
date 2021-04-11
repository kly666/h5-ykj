<template>
  <div id="app">
    <Head />
    <Main />
    <Floor />
    <Menu />
    <PageDownload />
    <Footer />
  </div>
</template>

<script>
import Head from "views/Head/Head";
import Main from "views/Main/Main";
import Floor from "views/Floor/Floor";
import Menu from "views/Footer/Menu";
import PageDownload from "views/Footer/PageDownload";
import Footer from "views/Footer/Footer";

export default {
  name: "App",
  components: {
    Head,
    Main,
    Floor,
    Menu,
    PageDownload,
    Footer,
  },

  // beforeCreate() {
  //   if (
  //     !navigator.userAgent.match(
  //       /(phone|pad|pod|iPhone|iPod|ios|iPad|Android|Mobile|BlackBerry|IEMobile|MQQBrowser|JUC|Fennec|wOSBrowser|BrowserNG|WebOS|Symbian|Windows Phone)/i
  //     )
  //   ) {
  //     window.location.href = "https://www.baidu.com"; //电脑
  //   }
  // },
};
</script>

<style>
@import "assets/css/normalize.css";
</style>
