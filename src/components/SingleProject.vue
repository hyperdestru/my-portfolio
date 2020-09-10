<template>
	<v-row 
		justify="center" 
		class="single-project"
	>
		<v-col 
			cols="10" 
			class="
				d-flex 
				flex-row 
				justify-center
			"
		>

			<single-thumbnail>
			</single-thumbnail>

			<project-details
				:title="project.title"
				:description="project.description"
				:stack="project.stack"
			>
			</project-details>
		</v-col>
	</v-row>
</template>

<script>
import SingleThumbnail from './SingleThumbnail'
import ProjectDetails from './ProjectDetails'

export default {
	name: 'SingleProject',

	components: {
		'single-thumbnail': SingleThumbnail,
		'project-details': ProjectDetails
	},

	props: {
		project: {
			type: Object,
			required: true
		}
	}
}
</script>