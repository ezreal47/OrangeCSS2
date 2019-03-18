<template>
  <div class="collapse">
    <slot></slot>
  </div>
</template>

<script>
export default {
  
}
</script>

<style lang="scss" scoped>
  .collapse {
    border-radius: 4px;
    border: 1px solid #dcdee2;
    max-width: 700px;
    overflow: hidden;
  }
</style>