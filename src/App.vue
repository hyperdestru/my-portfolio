<template>
	<v-app>
		<v-main>
			<the-header></the-header>
			<v-container>
				<the-banner></the-banner>
				<the-projects></the-projects>
				<the-testimonies></the-testimonies>
				<the-contact></the-contact>
			</v-container>
			<the-footer></the-footer>
		</v-main>
	</v-app>
</template>

<script>
import TheHeader from './views/TheHeader'
import TheFooter from './views/TheFooter'
import TheBanner from './views/TheBanner'
import TheProjects from './views/TheProjects'
import TheTestimonies from './views/TheTestimonies'
import TheContact from './views/TheContact'

export default {
	name: 'App',

	components: {
		'the-header': TheHeader,
		'the-footer': TheFooter,
		'the-banner': TheBanner,
		'the-projects': TheProjects,
		'the-testimonies': TheTestimonies,
		'the-contact': TheContact
	}
}
</script>