<template>
<FixedHeader :threshold="10">
  <div class="nav px-3">
    <div class="nav-header">
<div class="nav-title">
        <img src="../assets/logo.svg" alt="Mi café ideal" class="img-logo float-left">          
      </div>
    </div>
    <div class="nav-btn">
      <label for="nav-check">
        <span></span>
        <span></span>
        <span></span>
      </label>
    </div>
    <input type="checkbox" id="nav-check">
    <div class="nav-links">
      <a target="_blank">Suscripción de café</a>
      <a target="_blank">Comprar café</a>
      <a target="_blank">Souvenirs</a>
      <a target="_blank">Nuestro café</a>
      <a class="btn-subscribe btn-aqua b-aqua bold">Encuentra tu café ideal</a>        
    </div>
  </div>
</FixedHeader>
</template>

<script>
import FixedHeader from 'vue-fixed-header'
export default {
  components: {
    FixedHeader
  },
  data() {
    return {
      isFixed: true
    }
  }
}
</script>
<style scoped>
.nav {
  height: 80px;
  width: 100%;
  /* background-color: #4d4d4d; */
  background-color: rgba(23, 2, 32, 0.71);

  position: relative;
}

.nav > .nav-header {
  display: inline;
}

.nav > .nav-header > .nav-title {
  display: inline-block;
  font-size: 22px;
  color: #fff;
  padding-top: 5px;
  padding-bottom: 5px;
}

.nav > .nav-header > .nav-title > img {
  width: 100%;
}

.nav > .nav-btn {
  display: none;
}

.nav > .nav-links {
  display: inline;
  float: right;
  font-size: 18px;
}

.nav > .nav-links > a {
  display: inline-block;
  padding: 25px 10px 25px 10px;
  text-decoration: none;
  color: #efefef;
  transition: 1s;
  -webkit-transition: 1s;
}

.nav > .nav-links > a:hover {
  background-color: rgba(0, 0, 0, 0.3);
}

.nav > #nav-check {
  display: none;
}

@media (max-width: 909px) {
  .nav {
    height: 50px;
  }
  .nav > .nav-header > .nav-title > img {
    width: 65%;
  }
  .nav .btn-subscribe {
    width: 256px !important;
  }
  .nav > .nav-btn {
    display: inline-block;
    position: absolute;
    right: 0px;
    top: 0px;
  }
  .nav > .nav-btn > label {
    display: inline-block;
    width: 50px;
    height: 50px;
    padding: 13px;
  }
  .nav > .nav-btn > label:hover {
    background-color: rgba(0, 0, 0, 0.3);
  }
  .nav > .nav-btn > label > span {
    display: block;
    width: 25px;
    height: 10px;
    border-top: 2px solid #eee;
  }
  .nav > .nav-links {
    position: absolute;
    display: block;
    width: 100%;
    background-color: #333;
    height: 0px;
    transition: all 0.3s ease-in;
    overflow-y: hidden;
    top: 50px;
    left: 0px;
    padding: 0px 20px;
    z-index: 10;
  }
  .nav > .nav-links > a {
    display: block;
    width: 100%;
  }
  .nav > #nav-check:not(:checked) + .nav-links {
    height: 0px;
  }
  .nav > #nav-check:checked + .nav-links {
    height: calc(100vh - 50px);
    overflow-y: auto;
  }
}
</style>
