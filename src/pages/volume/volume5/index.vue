<template>
  <div class="box">
    <vlhead></vlhead>
    <p>当前第5题/共8题</p>
    <span>5.你希望通过学习获得哪些方面的改变?(填空题)</span>

    <textarea cols="30" rows="10" placeholder="请提出你的宝贵意见"></textarea>

    <div class="volume1but" @click="JumpVl6">下一题</div>
  </div>
</template>

<script>
import vlhead from "../../../components/volhead";
export default {
  props: {},
  data() {
    return {};
  },
  computed: {},
  created() {},
  mounted() {},
  watch: {},
  methods: {
    JumpVl6() {
      mpvue.navigateTo({ url: "../volume6/main" });
    }
  },
  components: {
    vlhead
  }
};
</script>


<style>
.box span {
  font-weight: 700;
  margin-left: 20rpx;
}
.box p {
  margin: 20rpx 0rpx 20rpx 40rpx;
}

.volume1but {
  text-align: center;
  width: 400rpx;
  margin: 50rpx auto;
  padding: 20rpx;
  background-color: rgb(81, 169, 51);
  color: white;
  border-radius: 15rpx;
}
textarea{
  border: 1rpx solid #7777;
  border-radius: 10rpx;
  padding: 30rpx;
  margin: 20rpx auto;
}
</style>