<template>
  <div class="main">
    <Header></Header>
    <Section1></Section1>
    <!-- <div class="container"> -->
    <Section2></Section2>      
    <!-- </div> -->
  </div>
</template>
<script>
import Header from '../components/Header'
import Section1 from '../components/Section1'
import Section2 from '../components/Section2'
export default {
  data() {
    return {}
  },
  components: {
    Header,
    Section1,
    Section2
  }
}
</script>
<style>

</style>
