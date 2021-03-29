<template>
	<div 
		style="
			position: sticky;
			top: 0;
			z-index: 5;
		"
		class="
			d-flex
			flex-row
			justify-space-between
			align-center
			primary
		"
	>
		<header-logo>
		</header-logo>

		<classic-menu v-if="$vuetify.breakpoint.mdAndUp">
		</classic-menu>

		<dropdown-menu v-else-if="$vuetify.breakpoint.smAndDown">
		</dropdown-menu>
	</div>
</template>

<script>
import DropdownMenu from '@/components/DropdownMenu'
import ClassicMenu from '@/components/ClassicMenu'
import HeaderLogo from '@/components/HeaderLogo'

export default {
	name: 'TheHeader',

	components: {
		'dropdown-menu': DropdownMenu,
		'classic-menu': ClassicMenu,
		'header-logo': HeaderLogo
	}
}
</script>
