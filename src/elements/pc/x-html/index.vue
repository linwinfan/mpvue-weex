<template>
  <div class="pc-x-html" element-path="pc/x-html">
  {{viewModel}}
  </div>
</template>

<script>
  export default {
    name: 'x-html',
    props: {
      elementData: {}
    },
    data () {
      return {
        viewModel: ''
      }
    },
    mounted () {
      this.init()
    },
    methods: {
      async init () {
        if (this.elementData === undefined) {
          this.viewModel = this.elementData
        }
      }
    }
  }
</script>

<style lang="less">
  @import '~_style/index.less';
  .pc-x-html {
  	font-size: @font-size-base;
  }
</style>
