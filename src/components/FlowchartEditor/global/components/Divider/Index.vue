/**
*
* Divider
*/

<style scoped lang="scss">
  .divider {
    display: inline-block;
    background: rgba(0, 0, 0, 0.1);

    &.horizontal {
      width: 100%;
      height: 1px;
      margin: 5px auto;
    }
    &.vertical {
      width: 1px;
      height: 100%;
      margin: auto 5px;
    }
  }
</style>

<template>
  <div :class="['divider', mode]"></div>
</template>

<script>
  export default {
    name: 'Divider',
    props: {
      mode: {
        type: String,
        // 水平还是垂直类型，可选值为 horizontal 或 vertical
        default: 'horizontal'
      }
    }
  }
</script>
