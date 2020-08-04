<template>
	<div 
		style="height: 600px"
		class="
			d-flex 
			flex-column 
			justify-space-around
			align-center
		"
	>
		<div class="text-center text-uppercase">
			<h2 class="text-h1">
				{{ $t('messages.tBanner') }}
			</h2>
			<h1 class="text-h6 py-4" style="letter-spacing: .4rem">
				{{ $t('messages.stBanner') }}
			</h1>
		</div>

		<scroll-cta>
		</scroll-cta>
	</div>
</template>

<script>
	import ScrollCta from './ScrollCta'

	export default {
		name: 'TheBanner',

		components: {
			'scroll-cta': ScrollCta
		}
	}
</script>
