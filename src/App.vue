<template>
  <div id="app">
    <img src="@/assets/malu.jpg" alt class="bg" />
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
.bg {
  width: 100%;
  height: 100%;
  opacity: 0.75;
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: -1;
}
</style>
