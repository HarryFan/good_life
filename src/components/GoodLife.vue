<template>
  <!-- 使用 Vue 的模板語言 -->
  <div class="container">
    <h3>好文</h3>
    <ul>
      <!-- 使用 v-for 指令渲染列表 -->
      <li v-for="(item, index) in items" :key="index">
        <h4>{{ item.title }}</h4>
        <p>{{ item.quote }}</p>
      </li>
    </ul>
  </div>
</template>
<script>
  // 導入 contents.json 文件
  import contents from '../json/contents.json'

  export default {
    // 設置名稱為 GoodLife 的 Vue 組件
    name: 'GoodLife',
    data() {
      // 定義 items 數據
      return {
        items: contents
      }
    }
  }
</script>
<style scoped lang="scss">
  /* 使用 Sass */
  .container {
    position: relative;
    margin: 0 auto;
    max-width: 960px;
    text-align: center;

    li {
      margin: 30px auto;
      position: relative;
      list-style-type: none;
    }
  }
</style>
