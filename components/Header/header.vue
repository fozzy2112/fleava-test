<template>
	<section>
		<h2>Flickity</h2>
		<flickity  class="flickity" ref="flickity" :options="flickityOptions">
			<div class="carousel-cell">
				<img src="https://via.placeholder.com/150" style="width:100%" alt="">
			</div>
			<div class="carousel-cell">
				<img src="https://via.placeholder.com/150" style="width:100%" alt="">
			</div>
			<div class="carousel-cell">
				<img src="https://via.placeholder.com/150" style="width:100%" alt="">
			</div>
			<div class="carousel-cell">
				<img src="https://via.placeholder.com/150" style="width:100%" alt="">
			</div>
			<div class="carousel-cell">
				<img src="https://via.placeholder.com/150" style="width:100%" alt="">
			</div>
		</flickity>
	</section>
</template>

<script>
import Flickity from 'vue-flickity'
export default {
	components : {
		Flickity
	},
	data() {
		return {
			flickityOptions: {
				initialIndex: 3,
				prevNextButtons: true,
				pageDots: true,
				wrapAround: true,
				freeScroll: true
				// any options from Flickity can be used
			}
		}
	}
}
</script>

<style>
.carousel-cell {
  width: 100%; /* full width */
  height: 160px; /* height of carousel */
  margin-right: 10px;
}
</style>