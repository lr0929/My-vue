<template>
	<div class="aboutus">
		<div class="swiper-container">
			<div class="swiper-wrapper">
				<div class="swiper-slide">Slide 1</div>
				<div class="swiper-slide">Slide 2</div>
				<div class="swiper-slide">Slide 3</div>
				<div class="swiper-slide">Slide 4</div>
				<div class="swiper-slide">Slide 5</div>
				<div class="swiper-slide">Slide 6</div>
				<div class="swiper-slide">Slide 7</div>
			</div>
			<!-- Add Pagination -->
			<!-- <div class="swiper-pagination"></div> -->
		</div>
	</div>
</template>

<script>
	import Swiper from "swiper"
	export default {
		name: 'index',
		data() {
			return {

			}
		},
		created() {
		},
		mounted() {
            this.myswipery()

		},
		methods: {
			myswipery: function() {
				var swiper = new Swiper('.swiper-container', {
					direction: 'vertical',
					slidesPerView: 1,
					spaceBetween: 30,
					mousewheel: true,
					pagination: {
						el: '.swiper-pagination',
						clickable: true,
					},
				});
			},
		}
	}
</script>

<style>
	@import url("../../node_modules/swiper/css/swiper.css");
	.aboutus {
		height: 14rem;
	}
	   .swiper-container {
	        width: 100%;
	        height: 100%;
	        margin-left: auto;
	        margin-right: auto;
	    }
	    .swiper-slide {
	        text-align: center;
	        font-size: 18px;
	        background: #fff;
	
	        /* Center slide text vertically */
	        display: -webkit-box;
	        display: -ms-flexbox;
	        display: -webkit-flex;
	        display: flex;
	        -webkit-box-pack: center;
	        -ms-flex-pack: center;
	        -webkit-justify-content: center;
	        justify-content: center;
	        -webkit-box-align: center;
	        -ms-flex-align: center;
	        -webkit-align-items: center;
	        align-items: center;
	    }
</style>
