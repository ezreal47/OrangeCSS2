<template>
  <div id="app">  
    <!--<o-button>默认按钮</o-button>
    <o-button type="primary" @click="name">Primary</o-button>
    <o-button type="success">Success</o-button>
    <o-button type="error">Error</o-button>
    <o-button icon="search">搜索按钮</o-button>
    <o-button icon="download">下载按钮</o-button>
    <o-button size="large">Large</o-button>
    <o-button size="small">small</o-button>
    <o-button :loading="true">Loading</o-button>
    <o-input disabled></o-input>
    <o-input search></o-input>
    <o-input search enter-button></o-input>
    <div @click="name">aaaaaaaaaaa</div>

    <o-row gutter="20">
      <o-col span="4" order="4">1</o-col>
      <o-col span="8" order="2">2</o-col>
      <o-col span="2" order="1">3</o-col>
      <o-col span="4" order="3">4</o-col>
    </o-row>

    <button @click="info('这是一条普通的消息')">提示消息</button>
    <o-button @click="success('这是一条成功的消息')">成功消息</o-button>
    <o-button @click="error('抛出一个的错误信息')">错误消息</o-button>
    <o-button @click="warning('抛出一个的警告信息!')">警告消息</o-button>


    <o-tab selected="React">
      <o-tab-head>
        <o-tab-item name="Vuea">Vue</o-tab-item>
        <o-tab-item name="React">React</o-tab-item>
        <o-tab-item name="Angulart" disabled>ANGULLARA</o-tab-item>
      </o-tab-head>

      <o-tab-body>
        <o-tab-pane name="Vuea">Tab1的内容</o-tab-pane>
        <o-tab-pane name="React">Tab2</o-tab-pane>
        <o-tab-pane name="Angulart">Tab3的内容</o-tab-pane>
      </o-tab-body>
    </o-tab>-->
    
  
    <!--<o-popover trigger="click">
      <template slot="content">
        <div>popover内容</div>
      </template>
      <o-button type="primary">click</o-button>
    </o-popover>

    <o-popover position="bottom">
      <template slot="content">
        <div>popover内容</div>
      </template>
      <o-button>click</o-button>
    </o-popover>

 <o-popover position="top" trigger="hover">
      <template slot="content">
        <div>popover内容</div>
      </template>
      <o-button>click</o-button>
    </o-popover>

     <o-popover position="bottom" trigger="hover">
      <template slot="content">
        <div>popover内容</div>
      </template>
      <o-button>click</o-button>
    </o-popover>-->


  <!--<o-cascader :source="source" :selected="selected" @update:selected="selected = $event"></o-cascader>-->
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
<!--
     <o-carousel :selected.sync="sel" autoplay>  
      <carousel-item name="1">
        <div class="box">1</div>
      </carousel-item>
      <carousel-item name="2">
        <div class="box">2</div>
      </carousel-item>
      <carousel-item name="3">
        <div class="box">3</div>
      </carousel-item>
      <carousel-item name="4">
        <div class="box">4</div>
      </carousel-item>
    </o-carousel>-->
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {},
  data() {
    return {
      selected: [],
      sel: '',
      source: [
        {
          name: '广东省',
          children: [
            {
              name: '深圳市',
              children: [
                { name: '罗湖区' },
                { name: '福田区' },
                { name: "盐田区" },
                { name: "保安区" }
              ]
            },
            { name: '广州市' },
            {
              name: '东莞市',
              children: [
                { name: '樟木头镇' },
                { name: '东城区' },
                { name: '南城区' }
              ]
            }
          ]
        },
        {
          name: '浙江省',
          children: [
            {
              name: '杭州市',
              children: [
                { name: '上城区' },
                { name: '下城区' },
                { name: "江干区" },
                { name: "西湖" }
              ]
            },
            { name: '嘉兴' }
          ]
        }
      ]
    }
  },
  methods: {
    info(info) {
      this.$message.info(info)
    },
    success(info) {
      this.$message.success(info)
    },
    error(info) {
      this.$message.error(info)
    },
    warning(info) {
      this.$message.warning(info)
    }
  }
}
</script>

<style lang="scss">
#app {
  // .box {
  //     height: 300px;
  //     width: 700px;
  //     background-color: #46a1de;
  //     display: inline-flex;
  //     justify-content: center;
  //     align-items: center;
  //     color: #fff;
  //     font-size: 32px;
  //   }


  // font-family: 'Avenir', Helvetica, Arial, sans-serif;
  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
}
</style>
