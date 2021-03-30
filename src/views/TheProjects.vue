<template>
	<div id="the-projects" class="mt-10">
		<section-title :textContent="$t('sections.projects.title')">
		</section-title>

		<v-row v-for="(proj, index) in $t('projects')" :key="index">
			<single-project :project="proj">
			</single-project>
		</v-row>
	</div>
</template>

<script>
import SingleProject from '../components/SingleProject'
import SectionTitle from '../components/SectionTitle'

export default {
	name: 'TheProjects',

	components: {
		'single-project': SingleProject,
		'section-title': SectionTitle
	}
}
</script>