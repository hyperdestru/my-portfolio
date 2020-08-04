<template>
	<the-banner></the-banner>
</template>

<script>
	import TheBanner from '../components/TheBanner'

	export default {
		name: 'TheHome',

		components: {
			'the-banner': TheBanner,
		}
	}
</script>