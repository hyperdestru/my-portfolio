<template>
	<v-col cols="4" class="project-details-content">
		<h3>
			{{ title }}
		</h3>
		<p>
			{{ description }}
		</p>
	</v-col>
</template>

<script>
export default {
	name: 'ProjectDetails',

	props: {
		title: String,
		description: String
	}
}
</script>