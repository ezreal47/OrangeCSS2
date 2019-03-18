<template>
  <div>
    <o-popover trigger="click">
      <template slot="content">
        <div>popover内容</div>
      </template>
      <o-button type="primary">click激活</o-button>
    </o-popover>

    <o-popover trigger="hover">
      <template slot="content">
        <div>popover内容</div>
      </template>
      <o-button>hover激活</o-button>
    </o-popover>

    <div class="box">
      <o-popover trigger="hover" position="top">
        <template slot="content">
          <div>popover内容</div>
        </template>
        <o-button type="primary">top</o-button>
      </o-popover>

      <o-popover trigger="hover" position="bottom">
        <template slot="content">
          <div>popover内容</div>
        </template>
        <o-button>bottom</o-button>
      </o-popover>

      <div class="box2">
        <o-popover trigger="hover" position="left">
          <template slot="content">
            <div>popover内容</div>
          </template>
          <o-button type="primary">left</o-button>
        </o-popover>
        <o-popover trigger="hover" position="right">
          <template slot="content">
            <div>popover内容</div>
          </template>
          <o-button>right</o-button>
        </o-popover>
      </div>
    </div>
<pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import Popover from '../../../src/components/popover'
import Button from '../../../src/components/button'
export default {
  components: {
    'o-popover': Popover,
    'o-button': Button
  },
  data() {
    return {
      content: `
<o-popover trigger="click">
  <template slot="content">
    <div>popover内容</div>
  </template>
  <o-button type="primary">click激活</o-button>
</o-popover>
<o-popover trigger="hover">
  <template slot="content">
    <div>popover内容</div>
  </template>
  <o-button>hover激活</o-button>
</o-popover>

<o-popover trigger="hover" position="top">
  <template slot="content">
    <div>popover内容</div>
  </template>
  <o-button type="primary">top</o-button>
</o-popover>
<o-popover trigger="hover" position="bottom">
  <template slot="content">
    <div>popover内容</div>
  </template>
  <o-button>bottom</o-button>
</o-popover>
`.trim()
    }
  }
}
</script>
<style lang="scss" scoped>
  .box {
    margin: 20px 0;
    .box2 {
      margin: 20px 0;
    }
  }
</style>
