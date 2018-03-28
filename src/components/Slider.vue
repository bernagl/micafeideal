<template>
<div class="row mt-3 mb-5 my-md-0">
    <div class="col-12 col-lg-12 mb-3 text-center text-lg-left">
      <h3 class="c-white">¿Qué tan fuerte lo prefieres?</h3>
    </div>
    <div class="col-12 col-lg-10 my-2">
        <input type="range" id="slider" name="slider"> 
        <!-- <output for="slider" onforminput="value = slider.valueAsNumber;"></output> -->
    </div>
    <div class="col-12 col-lg-10 mt-2 text-center">
      <div class="row justify-content-center">
        <div class="col-6">
          <a class="btn-continuar btn-aqua b-aqua bold d-block fs-16">Continuar <i class="icon icon-chevron-right"></i></a>  
        </div>
      </div>
    </div>
</div>
</template>
<style scoped>
.btn-continuar {
  width: 100% !important;
}
#slider {
  -webkit-appearance: none;
  width: 100%;
  height: 30px;
  border-radius: 50px;
  outline: none;
  opacity: 0.7;
  -webkit-transition: 0.2s;
  transition: opacity 0.2s;

  background: -moz-linear-gradient(
    53deg,
    rgba(156, 138, 132, 1) 0%,
    rgba(128, 44, 25, 1) 100%
  ); /* ff3.6+ */
  background: -webkit-gradient(
    linear,
    left bottom,
    right top,
    color-stop(0%, rgba(156, 138, 132, 1)),
    color-stop(100%, rgba(128, 44, 25, 1))
  ); /* safari4+,chrome */
  background: -webkit-linear-gradient(
    53deg,
    rgba(156, 138, 132, 1) 0%,
    rgba(128, 44, 25, 1) 100%
  ); /* safari5.1+,chrome10+ */
  background: -o-linear-gradient(
    53deg,
    rgba(156, 138, 132, 1) 0%,
    rgba(128, 44, 25, 1) 100%
  ); /* opera 11.10+ */
  background: -ms-linear-gradient(
    53deg,
    rgba(156, 138, 132, 1) 0%,
    rgba(128, 44, 25, 1) 100%
  ); /* ie10+ */
  background: linear-gradient(
    37deg,
    rgba(156, 138, 132, 1) 0%,
    rgba(128, 44, 25, 1) 100%
  ); /* w3c */
  filter: progid:DXImageTransform.Microsoft.gradient(
      startColorstr='#802C19',
      endColorstr='#9C8A84',
      GradientType=0
    ); /* ie6-9 */
}

#slider:hover {
  opacity: 1;
}

#slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  appearance: none;
  width: 23px;
  height: 24px;
  border: 0;
  background: url('../assets/logo.png');
  background-size: contain;
  cursor: pointer;
}

#slider::-moz-range-thumb {
  width: 23px;
  height: 24px;
  border: 0;
  background: url('../assets/logo.png');
  background-size: contain;
  cursor: pointer;
}

output {
  position: absolute;
  background-image: linear-gradient(top, #444444, #999999);
  width: 40px;
  height: 30px;
  text-align: center;
  color: white;
  border-radius: 10px;
  display: inline-block;
  font: bold 15px/30px Georgia;
  bottom: 175%;
  left: 0;
  margin-left: -1%;
}
output:after {
  content: '';
  position: absolute;
  width: 0;
  height: 0;
  border-top: 10px solid #999999;
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  top: 100%;
  left: 50%;
  margin-left: -5px;
  margin-top: -1px;
}
</style>
