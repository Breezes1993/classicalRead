<template>
  <view class="content">
    <van-tree-select
      :items="items"
      :main-active-index="mainActiveIndex"
      @click-nav="onClickNav"
      @click-item="onClickItem"
	  class="tree-select"
	  height="100vh"
    >
      <view  slot="content" class="wrap">
		  <view>view</view>

	  </view>
    </van-tree-select>
  </view>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      title: "Hello",
      items: [{ text: 1 }, { text: 2 }],
      mainActiveIndex: 1
    };
  },
  onLoad() {},
  methods: {
    onClickNav(): void {},
    onClickItem(): void {}
  }
});
</script>

<style>
.tree-select .van-sidebar {
	width: 80rpx !important;
}
</style>
