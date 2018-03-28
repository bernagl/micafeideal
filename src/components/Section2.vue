<template>
<div class="section2 b-purple py-5">
    <div class="container">
        <div class="row">
            <div class="col-12 mb-5">
                <h2 class="text-center c-white">¿Por qué mi café ideal?</h2>
            </div>
            <div class="col-12">
                <div class="row justify-content-around">
                    <div class="col-12 my-3 my-md-0 col-md-4 text-center"
                    v-for="(image, key) in images" :key="key">
                        <DetailCard
                        :image="image.image" 
                        :text="image.title"
                        :title="image.text" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
</template>
<script>
import DetailCard from './DetailCard'
export default {
  components: { DetailCard },
  data() {
    return {
      images: [
        {
          image: 'img1.svg',
          title: 'Café de Altura',
          text: 'Te ofrecemos una selección de café de calidad.'
        },
        {
          image: 'img2.svg',
          title: 'Precio Justo',
          text: 'Te ofrecemos una selección de café de calidad.'
        },
        {
          image: 'img3.svg',
          title: 'Directo a tu casa',
          text: 'Te ofrecemos una selección de café de calidad.'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>


