<template>
	<div id="the-contact" class="mt-10">
		<section-title :textContent="$t('sections.contact.title')">
		</section-title>

		<v-list flat class="text-center">
			<v-list-item-group class="d-flex flex-row">
				<v-list-item 
					v-for="(page, index) in $t('contact')" 
					:key="index"
				>
					<v-list-item-content>
						<v-list-item-title class="secondary--text">
							{{ page.label }}
						</v-list-item-title>
					</v-list-item-content>
				</v-list-item>
			</v-list-item-group>
		</v-list>
	</div>
</template>

<script>
import SectionTitle from '../components/SectionTitle';

export default {
	name: 'TheContact',

	components: {
		'section-title': SectionTitle
	}
}
</script>