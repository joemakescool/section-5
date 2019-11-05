<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <template id="thing">
      <h1>{{ title }}</h1>
    </template>

  </div>
</template>

<script>

  setTimeout(()=> {
    console.log('Joe\'s message')
  }, 3000);

export default {
  name: 'app',
  components: {

  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
