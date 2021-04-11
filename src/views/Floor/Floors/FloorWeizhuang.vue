<template>
  <div class="floor_multi_type">
    <div class="w multi_type">
      <div class="top_room">
        <div class="all_type_icon">
          <img src="~assets/img/icon/weizhuang_icon.svg" alt="" />
        </div>
        <h1>应用伪装</h1>
        <h2>将你的秘密隐藏在精致的计算器</h2>
        <h2>/指南针/日历里</h2>
      </div>
      <div class="bottom_room">
        <img
          src="~assets/img/images/weizhuang_rili.png"
          alt=""
          class="first_img"
        />
        <img
          src="~assets/img/images/weizhuang_zhinanzhen.png"
          alt=""
          class="other_img"
        />
        <img
          src="~assets/img/images/weizhuang_jisuanqi.png"
          alt=""
          class="last_img"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FloorWeizhuang",
};
</script>

<style lang="less">
.floor_multi_type {
  padding-top: 25px;
  background-color: #ffffff;
  height: 500px;
  overflow: hidden;
  .multi_type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .bottom_room {
      position: relative;
      margin-top: 25px;
      background-color: #fff;
      text-align: center;
      img {
        width: 60%;
        border-radius: 20px;
      }
      .first_img {
        position: absolute;
        top: 30px;
        left: -10px;
      }
      .last_img {
        position: absolute;
        top: 30px;
        right: -10px;
      }
      .other_img {
        position: relative;
        z-index: 99;
      }
    }
    .top_room {
      display: flex;
      flex-direction: row;
      justify-content: center;
      flex-wrap: wrap;
      align-content: flex-start;
      padding-top: 40px;
      .all_type_icon {
        width: 400px;
        text-align: center;
        img {
          width: 60px;
          height: 60px;
        }
      }

      h1 {
        margin-top: 10px;
        font-size: 28px;
        font-weight: 400;
        color: #333;
      }
      h2 {
        width: 100%;
        text-align: center;
        margin-top: 10px;
        font-size: 20px;
        font-weight: 400;
        color: #666;
      }
    }
  }
}
</style>
