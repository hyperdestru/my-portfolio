<template>
	<v-list class="nav" flat>
		<v-list-item-group :class="{ 'd-flex': !dropdown }">
			<v-list-item 
				v-for="(page, index) in pages" 
				:key="index"
				@click="$vuetify.goTo(page.link)"
			>
				<v-list-item-content>
					<v-list-item-title>
						{{ page.name }}
					</v-list-item-title>
				</v-list-item-content>
			</v-list-item>
		</v-list-item-group>
	</v-list>
</template>

<script>
export default {
	name: 'TheNav',

	props: {
		dropdown: {
			type: Boolean,
			required: false
		}
	},

	data: () => ({
		pages: [
			{ name: 'Accueil', link: '#the-home' },
			{ name: 'Projets', link: '#the-projects' },
			{ name: 'A propos', link: '#the-about' },
			{ name: 'Contact', link: '#the-contact' }
		]
	})
}
</script>