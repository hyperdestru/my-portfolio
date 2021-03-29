<template>
	<v-app>
		<v-main>
			<the-header></the-header>
			<v-container>
				<the-home></the-home>
				<the-projects></the-projects>
				<the-about></the-about>
				<the-testimonies></the-testimonies>
				<the-contact></the-contact>
			</v-container>
			<the-footer></the-footer>
		</v-main>
	</v-app>
</template>

<script>
import TheHeader from './components/TheHeader'
import TheFooter from './components/TheFooter'
import TheHome from './views/TheHome'
import TheProjects from './views/TheProjects'
import TheAbout from './views/TheAbout'
import TheTestimonies from './views/TheTestimonies'
import TheContact from './views/TheContact'

export default {
	name: 'App',

	components: {
		'the-header': TheHeader,
		'the-footer': TheFooter,
		'the-home': TheHome,
		'the-projects': TheProjects,
		'the-about': TheAbout,
		'the-testimonies': TheTestimonies,
		'the-contact': TheContact
	}
}
</script>