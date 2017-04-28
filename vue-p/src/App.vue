<template>
  <div id="app">
    <h1 class="page-title">
      <a href="#/">开发组件库</a>
      <router-view></router-view>
    </h1>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style scoped>
@import './assets/css/App.css';
</style>
