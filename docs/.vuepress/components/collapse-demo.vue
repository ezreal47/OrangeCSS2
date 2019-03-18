<template>
  <div>
    <o-collapse>
        <panel>
            艾伦·麦席森·图灵
          <p slot="content">Alan Mathison Turing，英国数学家、逻辑学家，被称为计算机科学之父，人工智能之父。</p>
        </panel>
        <panel>
            斯蒂夫·盖瑞·沃兹尼亚克
            <p slot="content">Stephen Gary Wozniak曾就读于美国科罗拉多大学，后转学入美国著名高等学府加州大学伯克利分校（UC Berkeley）并获得电机工程及计算机（EECS）本科学位（1987年）。</p>
        </panel>
        <panel>
            尼古拉斯·泽卡斯
            <p slot="content">Nicholas C·Zakas是《Professional JavaScript for Web Developers | JavaScript高级程序设计》的作者。</p>
        </panel>
    </o-collapse>
  <pre><code>{{content}}</code></pre>
  </div>
</template>
<script>
import Collapse from '../../../src/components/collapse/collapse'
import CollapsePane from '../../../src/components/collapse/collapse-pane'
export default {
  components: {
    'o-collapse': Collapse,
    'panel': CollapsePane
  },
  data() {
    return {
      content: `
<o-collapse>
  <panel>
    艾伦·麦席森·图灵
    <p slot="content">Alan Mathison Turing，英国数学家、逻辑学家，被称为计算机科学之父，人工智能之父。</p>
  </panel>
  <panel>
    斯蒂夫·盖瑞·沃兹尼亚克
    <p slot="content">Stephen Gary Wozniak曾就读于美国科罗拉多大学，后转学入美国著名高等学府加州大学伯克利分校（UC Berkeley）并获得电机工程及计算机（EECS）本科学位（1987年）。</p>
  </panel>
  <panel>
    尼古拉斯·泽卡斯
    <p slot="content">Nicholas C·Zakas是《Professional JavaScript for Web Developers | JavaScript高级程序设计》的作者。</p>
  </panel>
</o-collapse>    
`.trim()
    }
  }

}
</script>