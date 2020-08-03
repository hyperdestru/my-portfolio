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
		<div class="text-center">
			<img 
				src="../assets/logo-black-green.png"
				alt="Gaël Dumon"
			>
			<p class="text-uppercase mr-9 py-4 ma-0" style="letter-spacing: .4rem">
				{{ $t('messages.stBanner') }}
			</p>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'TheBanner'
	}
</script>
