<template>
<div class="section1">
    <div class="container">
        <div class=" row justify-content-between py-md-5 py-2">
            <div class="col-12 col-md-6">
                <div class="row">
                    <div class="col-12 hidden-xs-down">
                        <h1 class="c-white main-title">Encuentra el café que más te gusta.</h1>
                        <h2 class="c-aqua second-title">Suscríbete y recíbelo en casa.</h2>
                    </div>
                    <div class="col-12 mt-5">
                      <Slider></Slider>
                    </div>
                </div>
            </div>
            <div class="col-12 col-md-5 col-lg-4 col-xl-3 align-self-end">
                <CoffeCard></CoffeCard>
            </div>
        </div>
    <div class="div-background">
    </div>
    </div>
</div>
</template>
<script>
import CoffeCard from '@/components/CoffeCard'
import Slider from '@/components/Slider'
export default {
  components: { CoffeCard, Slider }
}
</script>

<style scoped>
.section1 {
  height: calc(100vh - 80px);
  background-color: rgba(48, 8, 67, 0.71);
}
.div-background {
  position: fixed;
  top: 0px;
  left: 0px;
  right: 0px;
  z-index: -1;
  /* background-color: rgba(185, 178, 178, 0.71); */
  background-image: url('http://www.cafebrasileiro.pl/wp-content/uploads/2015/08/ziarno-kawy.jpg');
  background-size: cover;
  min-height: calc(100vh - 80px);}

.main-title {
  font-size: 48px !important;
}
.second-title {
  font-size: 34px !important;
}
</style>


