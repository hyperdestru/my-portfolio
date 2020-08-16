<template>
	<v-container fluid id="the-projects">
		<h3 class="text-center">
			{{ $t('messages.tProjects') }}
		</h3>
		<v-row v-for="(proj, index) in $t('projects')" :key="index">
			<single-project :project="proj">
			</single-project>
		</v-row>
	</v-container>
</template>

<script>
import SingleProject from '../components/SingleProject'

export default {
	name: 'TheProjects',

	components: {
		'single-project': SingleProject,
	}
}
</script>