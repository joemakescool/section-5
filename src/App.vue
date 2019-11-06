<template>
  <div id="app">

    <img alt="Vue logo" src="./assets/logo.png">
    <template id="thing">
      <h1>{{ title }}</h1>
      <button @click="title = 'Changed'">Update Title</button>
      <button @click="destroy">Destroy</button>
    </template>
  </div>
</template>




<script>


export default {
  name: 'app',
  components: {

  },

  data: () => ({
    title: 'Joe\'s life cycle!'

  }),

  beforeCreate: function() {
    // eslint-disable-next-line no-console
    console.log('beforeCreate()')
  },

  created: function () {
    // eslint-disable-next-line no-console
    console.log('created()')
  },

  beforeMount: function () {
    // eslint-disable-next-line no-console
    console.log('beforeMount()')
  },

  mounted: function() {
    // eslint-disable-next-line no-console
    console.log('mounted()')
  },

  beforeUpdate: function() {
    // eslint-disable-next-line no-console
    console.log('beforeUpdate()')
  },

  updated: function() {
    // eslint-disable-next-line no-console
    console.log('updated()')
  },

  beforeDestroy: function() {
    // eslint-disable-next-line no-console
    console.log('beforeDestroy()')
  },

  destoryed: function() {
    // eslint-disable-next-line no-console
    console.log('destroyed()')
  },

  methods: {
    destroy: function () {
      this.$destroy();
    }
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
