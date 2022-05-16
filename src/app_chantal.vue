<template>
  <!-- <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> 
  </div> -->

 <!-- <div id = "app">
    <p :style="{'background-color': primaryColor}">{{ firstName }}</p>
    <p :style="primaryStyling">{{ firstName }}</p>
    <img 
      v-bind:src="imgLink"
    >
  </div> -->

  <div id="vue-app">
    <h1>Conditionals</h1>
    <button v-on:click="error = !error">Toggle Error</button>
    <button v-on:click="success = !success">Toggle Success</button> 
    <p v-if="error">There has been an error</p>
    <p v-else-if="success">Whoo, success>


  </div>

</template>

<script>
/*import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
} */

/*export default {
  name: "App",
  data() {
    return {
      firstName: "Chantal",
      imgLink: require("../src/assets/chantal_logo.jpg"),
      primaryColor: "blue",
      primaryStyling: {
        color: "white",
        backgroundColor: "black",
      }
    };
  },
};*/

new Vue({
  el: 'vue-app',
  data: {
    error: false;
    success: false;
  }
})

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
