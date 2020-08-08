<template>
	<div>	
		<thumbnails-grid></thumbnails-grid>
	</div>
</template>

<script>
	import ThumbnailsGrid from './ThumbnailsGrid'

	export default {
		name: 'SingleProject',

		components: {
			'thumbnails-grid': ThumbnailsGrid
		}
	}
</script>