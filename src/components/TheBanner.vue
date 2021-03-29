<template>
	<div 
		:style="{ 'height': bannerHeight }"
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
			
			<h1 class="text-h6">
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
	},

	data: () => ({
		bannerHeight: `${(screen.height) - 164}px`
	})
}
</script>
