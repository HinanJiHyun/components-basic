<template>
  <div 
    :class="{large}"
    :style="{ backgroundColor: color }"
    class="btn">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      default: '#666'
    },
    large: {
      type: Boolean,
      default: false
    }
    // },
    // text: {
    //   type: String,
    //   default: ''
    // }
  }
}
</script>

<style scoped lang="scss">
  .btn{
    display: inline-block;
    margin: 4px;
    padding: 6px 12px;
    border-radius: 4px;
    background-color: #666;
    color: #fff;
    cursor: pointer;
    &.large{
      font-size: 20px;
      padding: 10px 20px;
    }
  }
</style>