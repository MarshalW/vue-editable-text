<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <div>
      <editable-text v-model="name" :placeholder="'姓名'" />
    </div>
    <div>结果：{{name}}</div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import EditableText from "./components/EditableText.vue";

export default {
  name: "app",
  components: {
    HelloWorld,
    EditableText
  },
  data() {
    return {
      name: ""
    };
  }
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
