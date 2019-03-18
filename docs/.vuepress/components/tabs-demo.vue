<template>
  <div>
    <o-tab selected="Tab1">
      <o-tab-head>
        <o-tab-item name="Tab1">One</o-tab-item>
        <o-tab-item name="Tab2">Two</o-tab-item>
        <o-tab-item name="Tab3">Three</o-tab-item>
        <o-tab-item name="Tab4" disabled>four</o-tab-item>
      </o-tab-head>

      <o-tab-body>
        <o-tab-pane name="Tab1">Tab1的内容</o-tab-pane>
        <o-tab-pane name="Tab2">Tab2的内容</o-tab-pane>
        <o-tab-pane name="Tab3">Tab3的内容</o-tab-pane>
        <o-tab-pane name="Tab4">Tab4的内容</o-tab-pane>
      </o-tab-body>
    </o-tab>
    <pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import TabHead from '../../../src/components/tabs/tab-head'
import TabBody from '../../../src/components/tabs/tab-body'
import TabItem from '../../../src/components/tabs/tab-item'
import TabPane from '../../../src/components/tabs/tab-pane'
import Tab from '../../../src/components/tabs/tab'
export default {
  components: {
    'o-tab': Tab,
    'o-tab-head': TabHead,
    'o-tab-body': TabBody,
    'o-tab-item': TabItem,
    'o-tab-pane': TabPane
  },
  data() {
    return {
      content: `
 <o-tab selected="Tab1">
      <o-tab-head>
        <o-tab-item name="Tab1">One</o-tab-item>
        <o-tab-item name="Tab2">Two</o-tab-item>
        <o-tab-item name="Tab3">Three</o-tab-item>
        <o-tab-item name="Tab4" disabled>four</o-tab-item>
      </o-tab-head>

      <o-tab-body>
        <o-tab-pane name="Tab1">Tab1的内容</o-tab-pane>
        <o-tab-pane name="Tab2">Tab2的内容</o-tab-pane>
        <o-tab-pane name="Tab3">Tab3的内容</o-tab-pane>
        <o-tab-pane name="Tab4">Tab4的内容</o-tab-pane>
      </o-tab-body>
</o-tab>
`.trim()
    }
  }
}
</script>