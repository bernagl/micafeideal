<template>
    <div class="section1" ref="section1">
        <div class="container">
            <div class=" row justify-content-between align-items-center py-md-0 pt-md-5 py-2">
                <div class="col-12 col-md-6">
                    <div class="row">
                        <div class="col-12 hidden-xs-down">
                            <h1 class="c-white main-title">Encuentra el café que más te gusta.</h1>
                            <h2 class="c-aqua second-title">Suscríbete y recíbelo en casa.</h2>
                        </div>
                        <div class="col-12 mt-0 mt-lg-5">
                        <Slider></Slider>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-5 col-lg-4 col-xl-3">
                    <CoffeCard></CoffeCard>
                </div>
            </div>
        <div class="div-background">
        </div>
        </div>
        <Polygonf position="bottomright-to-topright"></Polygonf>
    </div>
</template>
<script>
import CoffeCard from '@/components/CoffeCard'
import Polygonf from '@/components/Polygon'
import Slider from '@/components/Slider'
export default {
  components: { CoffeCard, Polygonf, Slider }
}
</script>

<style scoped>
.section1 {
  /* height: calc(100vh - 80px); */
  background-color: rgba(48, 8, 67, 0.71);
}
.div-background {
  position: fixed;
  top: 0px;
  left: 0px;
  right: 0px;
  z-index: -1;
  background-image: url('http://www.cafebrasileiro.pl/wp-content/uploads/2015/08/ziarno-kawy.jpg');
  background-size: cover;
  height: 100%;
}

.main-title {
  font-size: 48px !important;
}
.second-title {
  font-size: 34px !important;
}
</style>


