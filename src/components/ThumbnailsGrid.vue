<template>
	<v-col cols="4" class="thumbs-grid d-flex flex-wrap">
		<v-col cols="6" v-for="n in 4" :key="n">
			<thumbnail-solo >
			</thumbnail-solo>
		</v-col>
	</v-col>
</template>

<script>
	import ThumbnailSolo from './ThumbnailSolo'

	export default {
		name: "ThumbnailsGrid",

		components: {
			'thumbnail-solo': ThumbnailSolo
		}
	}
</script>