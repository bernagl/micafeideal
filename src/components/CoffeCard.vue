<template>
  <div class="coffe-card row justify-content-center text-center b-white pb-4 pt-2 mx-4 mx-md-0">
      <div class="col-12">
          <h3 class="c-lightpurple mb-4">{{ title }}</h3>
          <img src="https://www.cafescumbal.com/wp-content/uploads/2017/03/producto-bolsa1k-granseleccion.png" alt="">
          <h2 class="c-lightpurple mt-2">{{ name }}</h2>
          <div class="row align-items-center">
            <div class="col-6">
              <h2 class="title-after-price tached">$349</h2>
            </div>
            <div class="col-6">
              <span class="title-now-price bold">$249</span>
              <span>por mes.</span>
            </div>
            <div class="col-12 mt-4">
              <a class="bold btn-purple b-lightpurple px-4">Suscribirme<i class="icon icon-chevron-right"></i></a>
            </div>
          </div>
      </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      title: 'Suscripción ideal',
      name: 'Café Oaxaca'
    }
  }
}
</script>

<style>
.coffe-card {
  border-radius: 5px;
  opacity: 0.8;
}

img {
  width: 60%;
}
.tached {
  text-decoration: line-through;
}

.title-after-price {
  font-size: 32px;
}
.title-now-price {
  font-size: 38px;
}
</style>
