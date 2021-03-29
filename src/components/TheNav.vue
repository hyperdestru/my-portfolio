<template>
	<v-list class="nav primary" flat>
		<v-list-item-group :class="{ 'd-flex': !dropdown }">

			<v-list-item 
				v-for="(page, index) in pages" 
				:key="index"
				@click="$vuetify.goTo(page.link)"
			>
				<v-list-item-content>
					<v-list-item-title class="white--text">
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

	data: function() {
		return {
			pages: [
				{ 
					name: this.$i18n.t('nav.lHome'), 
					link: 0 
				},
				{ 
					name: this.$i18n.t('nav.lProjects'), 
					link: '#the-projects' 
				},
				{ 
					name: this.$i18n.t('nav.lAbout'), 
					link: '#the-about' 
				},
				{ 
					name: this.$i18n.t('nav.lTestimonies'), 
					link: '#the-testimonies' 
				},
				{ 
					name: this.$i18n.t('nav.lContact'), 
					link: '#the-contact' 
				}
			]
		}
	}
}
</script>