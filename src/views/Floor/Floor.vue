<template>
  <div id="floor">
    <FloorMultiType />
    <FloorUse class="bgcf7">
      <template v-slot:icon-img>
        <img src="~assets/img/icon/all_type_icon.svg" alt="" />
      </template>
      <template v-slot:title-h1> 全格式支持 </template>
      <template v-slot:title-h2> 给你的私密文件一个最隐秘的空间 </template>
      <template v-slot:img-2>
        <img src="~assets/img/images/all_type.png" alt="" />
      </template>
    </FloorUse>
    <FloorMimaben></FloorMimaben>
    <FloorUse class="bgcf7">
      <template v-slot:icon-img>
        <img src="~assets/img/icon/xiutan_icon.svg" alt="" />
      </template>
      <template v-slot:title-h1> 文件防嗅探 </template>
      <template v-slot:title-h2> 防止文件被非法应用/网站嗅探 </template>
      <template v-slot:img-2>
        <img src="~assets/img/images/xiutan.png" alt="" />
      </template>
    </FloorUse>
    <FloorWeizhuang></FloorWeizhuang>
    <FloorUse class="bgcf7">
      <template v-slot:icon-img>
        <img src="~assets/img/icon/huishou_icon.svg" alt="" />
      </template>
      <template v-slot:title-h1> 回收站 </template>
      <template v-slot:title-h2> 保存并恢复误删除的文件</template>
      <template v-slot:img-2>
        <img src="~assets/img/images/huishou.png" alt="" />
      </template>
    </FloorUse>
    <FloorJiami></FloorJiami>
  </div>
</template>

<script>
import FloorMultiType from "views/Floor/Floors/FloorMultiType";
import FloorUse from "views/Floor/Floors/FloorUse";
import FloorMimaben from "views/Floor/Floors/FloorMimaben";
import FloorWeizhuang from "views/Floor/Floors/FloorWeizhuang";
import FloorJiami from "views/Floor/Floors/FloorJiami";

export default {
  name: "Floor",
  components: {
    FloorMultiType,
    FloorUse,
    FloorMimaben,
    FloorWeizhuang,
    FloorJiami,
  },
};
</script>

<style>
.bgcf7 {
  background-color: #f7f7f7 !important;
}
</style>