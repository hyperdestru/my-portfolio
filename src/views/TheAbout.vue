<template>
	<div id="the-about">
		<h3 class="text-center">
			{{ $t('messages.tAbout') }}
		</h3>
		<v-card class="text-center">
			<v-card-text>
				{{ $t('messages.pAbout') }}
			</v-card-text>
		</v-card>
	</div>
</template>

<script>
export default {
	name: 'TheAbout'
}
</script>