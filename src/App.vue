<template>
	<v-app>
		<the-header>
		</the-header>
		<v-main>
			<the-home></the-home>
			<the-projects></the-projects>
			<the-about></the-about>
			<the-contact></the-contact>
		</v-main>
		<the-footer>
		</the-footer>
	</v-app>
</template>

<script>
import TheHeader from './components/TheHeader'
import TheFooter from './components/TheFooter'
import TheHome from './views/TheHome'
import TheProjects from './views/TheProjects'
import TheAbout from './views/TheAbout'
import TheContact from './views/TheContact'

export default {
	name: 'App',

	components: {
		'the-header': TheHeader,
		'the-footer': TheFooter,
		'the-home': TheHome,
		'the-projects': TheProjects,
		'the-about': TheAbout,
		'the-contact': TheContact
	}
}
</script>