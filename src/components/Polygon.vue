<template>
    <div :class="`polygon ${position}`"></div>
</template>

<script>
export default {
  props: ['color', 'position']
}
</script>

<style scoped>
.bottomright-to-topright {
	width: 100%;
	height: 40px;
	border-left: 98vw solid transparent;
	border-right: 0px solid transparent;
	border-bottom: 100px solid #300843;
}

.topleft-to-topright {
	width: 100%;
	height: 40px;
	border-right: 98vw solid transparent;
	/* border-right: 0px solid transparent; */
	border-top: 100px solid #300843;
}
</style>