<template>
	<div id="the-contact">
		<h3 class="text-center">
			{{ $t('messages.tContact') }}
		</h3>
		<v-card class="text-center">
			<v-list>
				<v-list-item-group>
					<v-list-item>
						<v-list-item-title>
							{{ $t('contact.email.label') }}
						</v-list-item-title>
					</v-list-item>

					<v-list-item>
						<v-list-item-title>
							{{ $t('contact.linkedin.label') }}
						</v-list-item-title>
					</v-list-item>

					<v-list-item>
						<v-list-item-title>
							{{ $t('contact.github.label') }}
						</v-list-item-title>
					</v-list-item>
				</v-list-item-group>
			</v-list>
		</v-card>
	</div>
</template>

<script>
export default {
	name: 'TheContact'
}
</script>