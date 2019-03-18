<template>
  <div>
    <o-row>
      <o-col span="12">50%</o-col>
      <o-col span="12">50%</o-col>
    </o-row>
    <o-row>
      <o-col span="8">33.33%</o-col>
      <o-col span="8">33.33%</o-col>
      <o-col span="8">33.33%</o-col>
    </o-row>
    <o-row>
      <o-col span="4">16.66%</o-col>
      <o-col span="6">25%</o-col>
      <o-col span="10">41.66%</o-col>
      <o-col span="4">16.66%</o-col>
    </o-row>
    <pre><code>{{content1}}</code></pre>

    
  </div>
</template>
<script>
import Row from '../../../src/components/row'
import Col from '../../../src/components/col'
export default {
  components: {
    'o-row': Row,
    'o-col': Col
  },
  data() {
    return {
      content1: `
<o-row>
  <o-col span="12">50%</o-col>
  <o-col span="12">50%</o-col>
</o-row>
<o-row>
  <o-col span="8">33.33%</o-col>
  <o-col span="8">33.33%</o-col>
  <o-col span="8">33.33%</o-col>
</o-row>
<o-row>
  <o-col span="4">16.66%</o-col>
  <o-col span="6">25%</o-col>
  <o-col span="10">41.66%</o-col>
  <o-col span="4">16.66%</o-col>
</o-row>
`.trim()
    }
  }
}
</script>