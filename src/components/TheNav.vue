<template>
	<v-list class="primary" flat>
		<v-list-item-group :class="{ 'd-flex': !dropdown }">
			<v-list-item 
				v-for="(page, index) in $t('nav')" 
				:key="index"
				@click="$vuetify.goTo(page.anchor)"
			>
				<v-list-item-content>
					<v-list-item-title class="white--text">
						{{ page.label }}
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
	}
}
</script>