<template>
  <div id="app">
    <!-- 3. add click and v-if = true into below -->
    <el-button type="primary" @click = "openDiag = true">Welcome</el-button>
    <!-- 1. bind a proporty -->
    <!-- add".sync", el- is a component, add sync to update in -->
    <el-dialog :visible.sync = "openDiag">
 
    <img src="./assets/logo.png">
    <div>
      <p>
        If Element is successfully added to this project, you'll see an
        <code v-text="'<el-button>'"></code>
        below
      </p>
      <el-button>el-button</el-button>
    </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "app",
  components: {
    HelloWorld,
    simba
  },
  data:function(){
    return {
      sendTreat: "Raw Hide",
      // 2. set false
      openDiag: false,
    }
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
