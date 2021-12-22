<template>
  <div id="app">
    <ModalRoot />
    <halo/>
   
  </div>
</template>

<script>
import ModalRoot from './modules/modals/components/ModalRoot.vue';

export default {
  name: 'App',
  components: { ModalRoot },

}
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