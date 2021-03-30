<template>
	<div id="the-testimonies" class="mt-10">
		<section-title :textContent="$t('sections.testimonies.title')">
		</section-title>

		<v-carousel v-model="model" hide-delimiters height="164">
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
import SectionTitle from '../components/SectionTitle'

export default {
	name: 'TheTestimonies',

	components: {
		'section-title': SectionTitle
	},

	data: function() {
		return {
			model: 0
		}
	}
}
</script>