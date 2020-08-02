<template>
	<v-app>
		<v-main>
			<the-banner></the-banner>
		</v-main>
	</v-app>
</template>

<script>
	import TheBanner from './components/TheBanner';

	export default {
		name: 'App',

		components: {
			'the-banner': TheBanner
		}
	}
</script>