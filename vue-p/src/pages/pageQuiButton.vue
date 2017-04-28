<template>
  <div id="pageQuiButton">
    <!--使用-->
    <qui-btn msg="确定" @btnClickEvent="doSth" class="small">
      <img slot="icon" class="ico" src="../assets/logo.png" alt="">
    </qui-btn>
  </div>
</template>

<script>
import quiBtn from '../components/quiButton.vue'  /* 引用 */
export default {
  name: 'pageQuiButton',
  components: {
    'qui-btn': quiBtn  /* 注册自定义标签 */
  },
  methods: {
    doSth: function () {
      alert('this is a btn')
    }
  }
}
</script> 

