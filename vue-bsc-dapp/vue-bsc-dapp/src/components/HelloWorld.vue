<!--
 * @Author: your name
 * @Date: 2021-09-22 16:20:58
 * @LastEditTime: 2021-09-23 16:58:59
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \vue-bsc-dapp\src\components\HelloWorld.vue
-->
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li>
        <a href="https://vuejs.org" target="_blank"> Core Docs </a>
      </li>
      <li>
        <a href="https://forum.vuejs.org" target="_blank"> Forum </a>
      </li>
      <li>
        <a href="https://chat.vuejs.org" target="_blank"> Community Chat </a>
      </li>
      <li>
        <a href="https://twitter.com/vuejs" target="_blank"> Twitter </a>
      </li>
      <br />
      <li>
        <a href="http://vuejs-templates.github.io/webpack/" target="_blank">
          Docs for This Template
        </a>
      </li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li>
        <a href="http://router.vuejs.org/" target="_blank"> vue-router </a>
      </li>
      <li>
        <a href="http://vuex.vuejs.org/" target="_blank"> vuex </a>
      </li>
      <li>
        <a href="http://vue-loader.vuejs.org/" target="_blank"> vue-loader </a>
      </li>
      <li>
        <a href="https://github.com/vuejs/awesome-vue" target="_blank">
          awesome-vue
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
import BscDapp from '@obsidians/bsc-dapp'
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
    };
  },
  mounted() {
    var bd = new BscDapp();
    var is = bd.isBrowserExtensionInstalled;
    debugger;
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
