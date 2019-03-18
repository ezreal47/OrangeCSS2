<template>
  <div>
    <o-button @click.native="info('这是一条普通的消息')">提示消息</o-button>
    <o-button @click.native="success('这是一条成功的消息')">成功消息</o-button>
    <o-button @click.native="error('抛出一个错误的信息')">错误消息</o-button>
    <o-button @click.native="warning('抛出一个警告的信息!')">警告消息</o-button>
<pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import Message from '../../../src/components/message'
import Button from '../../../src/components/button'
import Plugin from '../../../src/components/plugin'
import Vue from 'vue'

Vue.use(Plugin)

export default {
  components: {
    'o-button': Button
  },
  data() {
    return {
      content: `
<o-button @click.native="info('这是一条普通的消息')">提示消息</o-button>
<o-button @click.native="success('这是一条成功的消息')">成功消息</o-button>
<o-button @click.native="error('抛出一个的错误信息')">错误消息</o-button>
<o-button @click.native="warning('抛出一个的警告信息!')">警告消息</o-button>
`.trim()
    }
  },
   methods: {
    info(info){
      this.$message.info(info)
    },
    success(info){
      this.$message.success(info)
    },
    error(info){
      this.$message.error(info)
    },
    warning(info){
      this.$message.warning(info)
    }
  }
}
</script>