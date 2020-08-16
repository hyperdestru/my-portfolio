<template>
	<v-row justify="center" class="single-project">
		<v-col cols="10" class="single-project d-flex flex-row justify-center">	
			<thumbnails-grid>
			</thumbnails-grid>

			<project-details
				:title="project.title"
				:description="project.description"
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