<template>
	<div id="the-projects">
		<h3 class="text-center">
			{{ $t('messages.tProjects') }}
		</h3>
		<single-project></single-project>
	</div>
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