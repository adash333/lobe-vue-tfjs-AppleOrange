<template>
  <div id="app">
    <div class="main">
      <h1>Vue.js</h1>
      <img ref="img" src="./assets/AppleOrangeTensorFlowJS/example/apple.jpg" />
      <p>{{ msg }}</p>
      <button @click="orange()" class="btn-flat-border">Click!</button>
    </div>
    <footer class="footer"><a href="https://i-doctor.sakura.ne.jp/font/?p=45623">WordPressでフリーオリジナルフォント</a></footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      msg: "Hello Apple!"
    }
  },
  methods: {
    orange() {
      this.msg="Orange is coming!"
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin: 0;
  color: #2c3e50;
  display: flex; 
  flex-flow: column; 
  min-height: 100vh;
}
#app .main {
  flex: 1;
}
#app .footer {
  width: 100%;
  height: 40px; 
  flex:1;
  text-align: center;
  padding: 20px 0;
  background-color: #cccccc;
}
</style>