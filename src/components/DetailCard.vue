<template>
    <div class="text-center">
        <div class="row">
            <div class="col-12">
                <h4 class="c-white">{{ title }}</h4>                
            </div>
            <div class="col-12 my-3">
                <img :src="imgSrc" alt="">
            </div>
            <div class="col-12">
             <p class="c-aqua">Te ofrecemos una selección de café de calidad.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'DetailCard',
  props: ['image', 'text', 'title'],
  data() {
    return {
      imgSrc: require(`../assets/${this.image}`)
    }
  }
}
</script>
