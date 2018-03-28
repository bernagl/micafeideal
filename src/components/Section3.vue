<template>
    <div class="div-background">
        <Polygonf position="topleft-to-topright"></Polygonf>
        <div class="container">
            <div class="row justify-content-center history-container py-4">
                <div class="col-md-2 col-3">
                    <History></History>
                </div>
               <div class="col-md-2 col-3">
                    <History></History>
                </div>
                <div class="col-md-2 col-3">
                       <History></History>
                </div>
                <div class="col-md-2 col-3">
                    <History></History>
                </div>
             </div>
         </div>
        <Polygonf position="bottomright-to-topright"></Polygonf>    
    </div>
</template>

<script>
import Parallax from 'vue-parallaxy'
import History from '@/components/History'
import Polygonf from '@/components/Polygon'
export default {
  components: { History, Parallax, Polygonf }
  //   data() {
  //     return { clientHeight: 99 }
  //   },
  //   computed: {
  //     setHeight: function() {
  //       return {
  //         'background-image':
  //           "url('http://greencappuccino.com/wp-content/uploads/2016/07/GettyImages502149672-1020x681.jpg')",
  //         'background-size': 'cover',
  //         height: '100%',
  //         position: 'fixed',
  //         top: this.clientHeight + 'px',
  //         right: 0,
  //         left: 0
  //       }
  //     }
  //   },
  //   mounted: function() {
  //     const s1 = document.getElementsByClassName('section1')[0].clientHeight
  //     const s2 = document.getElementsByClassName('section2')[0].clientHeight
  //     this.clientHeight = s1 + s2
  //   }
}
</script>

<style scoped>
.div-background {
  background-image: url('http://greencappuccino.com/wp-content/uploads/2016/07/GettyImages502149672-1020x681.jpg');
  background-size: cover;
  height: 100%;
}

.col-4 {
  min-height: 100px;
}
</style>