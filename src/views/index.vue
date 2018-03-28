<template>
  <div class="main">
    <Header></Header>
    <Section1></Section1>
    <!-- <div class="container"> -->
    <Section2></Section2>   
    <Section3></Section3>
    <Footer></Footer>     
    <!-- </div> -->
  </div>
</template>
<script>
import Footer from '../components/Footer'
import Header from '../components/Header'
import Section1 from '../components/Section1'
import Section2 from '../components/Section2'
import Section3 from '../components/Section3'
export default {
  data() {
    return {}
  },
  components: {
    Footer,
    Header,
    Section1,
    Section2,
    Section3
  }
}
</script>
<style>

</style>
