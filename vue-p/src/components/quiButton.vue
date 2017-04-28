<template>
  <button class="qui-btn">
    <slot name="icon"></slot>
    <span>{{msg}}</span>
  </button>
</template>

<script>
export default {
  props: {
    msg: {
      default: '下载'
    }
  },
  methods: {
    btnClickEvent: function () {
      alert(this.msg)
      this.$emit('btnClickEvent') /* 关键代码父组件触发自定义事件 */
    }
  }

}
</script>

<style scoped>
@import './css/reset.import.css';
@import './css/qui-btn.import.css';
</style>
