<template>
	<div class="my-4 text-h5 text-center primary white--text">
		{{ textContent.toUpperCase() }}
	</div>
</template>

<script>
export default {
	name: 'SectionTitle',

	props: {
		textContent: {
			required: true,
			type: String
		}
	}
}
</script>