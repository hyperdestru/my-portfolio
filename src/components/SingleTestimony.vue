<template>
	<v-card class="my-2 text-center">
		<v-card-text>
			{{ testimony.text }}
		</v-card-text>

		<v-card-subtitle>
			{{ testimony.author }}
		</v-card-subtitle>
	</v-card>
</template>

<script>
export default {
	name: 'SingleTestimony',

	props: {
		testimony: Object
	}
}
</script>