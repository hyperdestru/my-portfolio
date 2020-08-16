<template>
	<v-img
		:src="'https://picsum.photos/500/300?image=15'"
		:lazy-src="'https://picsum.photos/10/6?image=15'"
		aspect-ratio="1"
		class="thumb-solo grey lighten-2"
	>
		<template v-slot:placeholder>
			<v-row 
				class="fill-height ma-0" 
				align="center" 
				justify="center"
			>
				<v-progress-circular 
					indeterminate 
					color="grey lighten-5"
				>
				</v-progress-circular>
			</v-row>
		</template>
	</v-img>
</template>

<script>
	export default {
		name: 'ThumbnailSolo'
	}
</script>