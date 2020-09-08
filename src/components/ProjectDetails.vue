<template>
	<v-col cols="4" class="project-details-content">
		<h3>
			{{ title }}
		</h3>
		<p>
			{{ description }}
		</p>
		<ul>
			<li v-for="(tech, index) in stack" :key="index">
				{{ tech }}
			</li>
		</ul>
	</v-col>
</template>

<script>
export default {
	name: 'ProjectDetails',

	props: {
		title: String,
		description: String,
		stack: Array
	}
}
</script>