<template>
	<v-img
		:src="require(`../../assets/thumbnails/${projectSlug}.png`)"
		class="single-thumb grey lighten-2"
		max-width="350"
		max-height="348"
	>
		<template v-slot:placeholder>
			<v-row class="fill-height ma-0" align="center" justify="center">
				<v-progress-circular indeterminate color="grey lighten-5">
				</v-progress-circular>
			</v-row>
		</template>
	</v-img>
</template>

<script>
export default {
	name: 'SingleThumbnail',
	props: {
		projectSlug: {
			type: String,
			required: true
		}
	}
}
</script>