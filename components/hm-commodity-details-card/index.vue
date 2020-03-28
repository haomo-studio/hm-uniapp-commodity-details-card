<template>
  <div class="hm-commodity-details-card">
    <div class="box">
      <div><image class="item" :src="options.item" /></div>
      <div class="main">
        <text class="xiaomiBluetooth">{{ options.xiaomiBluetooth }}</text>
        <text class="count">{{ options.count }}</text>
        <text class="info">{{ options.info }}</text>
      </div>
      <div class="ft">
        <image
          class="xingtaiduICONxihuanHui"
          :src="options.xingtaiduICONxihuanHui"
        />
        <div class="originPriceWrap">
          <text class="price">{{ options.price }}</text>
          <text class="originPrice">{{ options.originPrice }}</text>
        </div>
        <image class="zujianguanli" :src="options.zujianguanli" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmCommodityDetailsCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-commodity-details-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          item:
            './images/img_25798_0_0.png',
          xiaomiBluetooth: '小米蓝牙',
          count: '4.0',
          info: '扬声器无线音频扬声器',
          xingtaiduICONxihuanHui:
            './images/img_25798_0_1.png',
          price: '¥89.95',
          originPrice: '¥115.95',
          zujianguanli:
            './images/img_25798_0_2.png'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
