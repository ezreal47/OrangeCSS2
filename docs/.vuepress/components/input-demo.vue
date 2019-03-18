<template>
  <div>
    <o-input></o-input>
    <o-input disabled></o-input>
    <o-input search></o-input>
    <o-input search enter-button></o-input>
    <pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import Input from '../../../src/components/input'
export default {
  components: {
    'o-input': Input
  },
  data() {
    return {
      content: `
<o-input></o-input>
<o-input disabled></o-input>
<o-input search></o-input>
<o-input search enter-button></o-input>
`.trim()
    }
  }
}
</script>