<template>
  <fixed-header :fixed.sync="isFixed" :threshold="100">
    <div :class="{ 'is-fixed': isFixed }">
      Your Content
    </div>
  </fixed-header>
</template>

<script>
import FixedHeader from 'vue-fixed-header'

export default {
  components: {
    FixedHeader
  },
  data() {
    return {
      isFixed: false
    }
  }
}
</script>