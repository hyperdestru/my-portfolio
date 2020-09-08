<template>
	<div id="the-testimonies">
		<h3 class="text-center">
			{{ $t('messages.tTestimonies') }}
		</h3>
		<single-testimony 
			v-for="(testimony, index) in $t('testimonies')" :key="index" 
			:testimony="testimony"
		>
		</single-testimony>
	</div>
</template>

<script>
import SingleTestimony from '../components/SingleTestimony'

export default {
	name: 'TheTestimonies',

	components: {
		'single-testimony': SingleTestimony
	}
}
</script>