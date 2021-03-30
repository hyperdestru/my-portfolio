<template>
	<div 
		:style="{ 'height': bannerHeight }"
		class="d-flex flex-column justify-space-around align-center"
	>
		<div class="text-center text-uppercase">
			<h2 class="text-h1">
				{{ $t('sections.banner.title') }}
			</h2>
			
			<h1 class="text-h6">
				{{ $t('sections.banner.subtitle') }}
			</h1>
		</div>

		<scroll-cta>
		</scroll-cta>
	</div>
</template>

<script>
import ScrollCta from '../components/ScrollCta'

export default {
	name: 'TheBanner',

	components: {
		'scroll-cta': ScrollCta
	},

	data: () => ({
		// For banner height I take the screen height minus 33% of that height
		bannerHeight: `${(screen.height - (screen.height * 0.33))}px`
	})
}
</script>
