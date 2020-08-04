<template>
	<v-app>
		<the-header></the-header>
		<v-main>
			<the-home></the-home>
		</v-main>
		<the-footer></the-footer>
	</v-app>
</template>

<script>
	import TheHeader from './components/TheHeader'
	import TheFooter from './components/TheFooter'
	import TheHome from './views/TheHome'

	export default {
		name: 'App',

		components: {
			'the-header': TheHeader,
			'the-footer': TheFooter,
			'the-home': TheHome
		}
	}
</script>