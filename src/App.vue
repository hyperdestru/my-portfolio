<template>
	<v-app>
		<the-header></the-header>
		<v-main>
			<the-banner></the-banner>
		</v-main>
	</v-app>
</template>

<script>
	import TheBanner from './components/TheBanner'
	import TheHeader from './components/TheHeader'

	export default {
		name: 'App',

		components: {
			'the-banner': TheBanner,
			'the-header': TheHeader
		}
	}
</script>