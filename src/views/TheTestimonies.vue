<template>
	<div id="the-testimonies" class="mt-10">
		<h3 class="text-center">
			{{ $t('messages.tTestimonies') }}
		</h3>
		<v-carousel v-model="model" hide-delimiters>
			<v-carousel-item
				v-for="(testimony, index) in $t('testimonies')"
				:key="index"
			>
				<v-sheet
					height="100%"
					color="white"
					tile
					class="
						secondary--text 
						d-flex 
						flex-column 
						align-center 
						justify-center
					"
				>
					<div class="text-center">
						<div class="display-1">
							{{ testimony.text }}
						</div>
						<div class="subtitle-1">
							{{ testimony.author }}
						</div>
					</div>
				</v-sheet>
			</v-carousel-item>
		</v-carousel>
	</div>
</template>

<script>
//import SingleTestimony from '../components/SingleTestimony'

export default {
	name: 'TheTestimonies',

	components: {
		//'single-testimony': SingleTestimony
	},

	data: function() {
		return {
			model: 0
		}
	}
}
</script>