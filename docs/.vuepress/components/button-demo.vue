<template>
  <div>
    <o-button>默认按钮</o-button>
    <o-button type="primary">Primary</o-button>
    <o-button type="success">Success</o-button>
    <o-button type="error">Error</o-button>
    <div class="box">
      <o-button icon="search">搜索按钮</o-button>
      <o-button icon="download">下载按钮</o-button>
      <o-button size="large">Large</o-button>
      <o-button size="small">small</o-button>
      <o-button :loading="true">Loading</o-button>
    </div>
    <pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import Button from '../../../src/components/button'
export default {
  components: {
    'o-button': Button
  },
  data() {
    return {
      content: `
<o-button>默认按钮</o-button>
<o-button type="primary">Primary</o-button>
<o-button type="success">Success</o-button>
<o-button type="error">Error</o-button>
<o-button icon="search">搜索按钮</o-button>
<o-button icon="download">下载按钮</o-button>
<o-button size="large">Large</o-button>
<o-button size="small">small</o-button>
<o-button :loading="true">Loading</o-button>
`.trim()
    }
  }
}
</script>
<style lang="scss" scoped>
  .box {
    margin-top: 20px;
  }
</style>
