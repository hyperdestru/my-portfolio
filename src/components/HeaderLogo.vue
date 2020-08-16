<template>
	<v-icon 
		x-large 
		@click="$vuetify.goTo('#the-home')"
	>
		mdi-code-braces-box
	</v-icon>
</template>

<script>
	export default {
		name: 'HeaderLogo'
	}
</script>

