<template>
		<div id="the-home">
			<the-banner>
			</the-banner>
		</div>
</template>

<script>
import TheBanner from '../components/TheBanner'

export default {
	name: 'TheHome',

	components: {
		'the-banner': TheBanner,
	}
}
</script>