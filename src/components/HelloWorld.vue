<template>
  <div class="hello">
    <div class="title">临时停车，请多关照</div>
    <div class="title-text">---致以真诚的歉意！</div>

    <img class="xin" src="@/assets/xin.jpg" alt />

    <div class="tel" @click="callPhone">一键电话挪车</div>

    <div class="footer">本页面为车主个人开发，仅供娱乐</div>
  </div>
</template>

<script>
import { Indicator } from "mint-ui";

export default {
  name: "phone",
  data() {
    return {};
  },
  methods: {
    callPhone() {
      window.location.href = "tel://13756835693";
    }
  }
};
</script>
<style scoped>
.footer {
  text-align: center;
  color: #f1f1f1;
  font-size: 0.5rem;
}
.tel {
  background-color: #ef4f4f;
  width: 9rem;
  height: 9rem;
  line-height: 9rem;
  border-radius: 50%;
  margin: 3rem auto 3rem;
  text-align: center;
  color: #fff;
  font-weight: 900;
  font-size: 1.2rem;
}

* {
  font-family: "楷体";
}

.title {
  font-size: 2rem;
  color: #333;
  text-align: center;
  height: 5rem;
  line-height: 7rem;
  font-weight: 700;
}
.title-text {
  font-size: 1rem;
  color: #666;
  text-align: right;
  height: 2rem;
  line-height: 2rem;
}
.xin {
  display: block;
  width: 96%;
  margin: 2rem auto 0;
  border-radius: 10px;
  box-shadow: 6px 6px 5px #999;
}
</style>
