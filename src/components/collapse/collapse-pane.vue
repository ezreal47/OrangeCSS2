<template>
  <div class="collapse-pane">
    <div class="title" @click="open = !open">
      <slot></slot>
    </div>
    <div class="content" v-if="open">
      <slot name="content"></slot>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      open: false
    }
  }
}
</script>

<style lang="scss" scoped>
.collapse-pane {
  .title {
    font-size: 14px;
    height: 38px;
    line-height: 38px;
    padding-left: 16px;
    color: #666;
    cursor: pointer;
    // position: relative;
    border: 1px solid #dcdee2;
    transition: all .2s ease-in-out;
    margin-top: -1px;
    margin-left: -1px;
    margin-right: -1px;
    display: flex;
    align-items: center;
    background-color: #f7f7f7;
  }
  .content {
    font-size: 14px;
    > p {
      padding: 0px 16px;
      margin: 6px 0;
    }
    color: #515a6e;
    background-color: #fff;
    margin: 0;
    padding: 0;
  }
}
</style>