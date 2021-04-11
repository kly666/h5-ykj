<template>
  <div class="floor_multi_type">
    <div class="multi_type">
      <div class="top_room">
        <div class="all_type_icon">
          <slot name="icon-img">
            <img src="~assets/img/icon/show_icon.svg" alt="" />
          </slot>
        </div>
        <h1>
          <slot name="title-h1"> 数据类别展示 </slot>
        </h1>
        <h2>
          <slot name="title-h2"> 让你的每一种私密文件得到安全保护 </slot>
        </h2>
      </div>
      <div class="bottom_room_use bgcf7 img70">
        <slot name="img-1" class="first_img">
          <!-- <img
            src="~assets/img/images/show_xiangce.png"
            alt=""
            class="first_img"
          /> -->
        </slot>
        <slot name="img-2" class="other_img">
          <!-- <img
            src="~assets/img/images/show_wenjiangui.png"
            alt=""
            class="other_img"
          /> -->
        </slot>
        <slot name="img-3" class="last_img">
          <!-- <img
            src="~assets/img/images/show_shipin.png"
            alt=""
            class="last_img"
          /> -->
        </slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FloorMultiType",
};
</script>

<style lang="less">
.floor_multi_type {
  padding-top: 25px;
  height: 420px;
  overflow: hidden;
  .multi_type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .bottom_room_use {
      position: relative;
      margin-top: 10px;
      // background-color: #f7f7f7;
      text-align: center;
      img {
        width: 70%;
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
      padding-top: 25px;
      .all_type_icon {
        width: 400px;
        text-align: center;
        img {
          width: 60px;
          height: 60px;
        }
      }

      h1 {
        text-align: center;
        width: 100%;
        margin-top: 10px;
        font-size: 28px;
        font-weight: 400;
        color: #333;
      }
      h2 {
        margin-top: 10px;
        font-size: 20px;
        font-weight: 400;
        color: #666;
      }
    }
  }
}
</style>
