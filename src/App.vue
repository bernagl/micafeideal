<template>
  <div>
  <Header></Header>
  <div class="container">
    <router-view/>
  </div>
  </div>
</template>

<script>
import Header from './components/header.vue'
export default {
  name: 'App',
  components: { Header }
}
</script>

<style>
@import 'at-ui-style';
@import 'bootstrap-4-grid';
</style>
