<template>
	<v-row justify="center" class="single-project">
		<v-col cols="10" class="d-flex flex-row justify-center">	
			<thumbnails-grid>
			</thumbnails-grid>

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
import ThumbnailsGrid from './ThumbnailsGrid'
import ProjectDetails from './ProjectDetails'

export default {
	name: 'SingleProject',

	components: {
		'thumbnails-grid': ThumbnailsGrid,
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