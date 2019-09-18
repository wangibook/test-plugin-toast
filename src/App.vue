<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>

    <button @click="handleClick">点击触发子组件的toast</button>
    <test-toast ref="toast"></test-toast>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {

    }
  },
  creted() {

  },
  methods: {
    handleClick() {
      this.$nextTick(() => {
        this.$refs.toast.toastPlugin('在父组件里触发调用的toast',2000)
      })
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
