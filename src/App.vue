<template>
  <div id="app">
    <my-header></my-header>
    <my-menu></my-menu>
    <my-main></my-main>
    <my-table></my-table>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Menu from './components/Menu.vue'
import Main from './components/Main.vue'
import Table from './components/Table.vue';

export default {
  name: 'App',
  components: {
    'my-header': Header,
    'my-menu': Menu,
    'my-main': Main,
    'my-table': Table
  },

}
</script>

<style>
  #app{
    font-family: 'Open-Sans';
  }
</style>
