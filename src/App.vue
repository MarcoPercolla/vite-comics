<script>
import AppHeader from './components/AppHeader.vue'
import AppComingSoon from './components/AppComingSoon.vue'
import AppProdotti from './components/AppProdotti.vue'
import AppFooter from './components/AppFooter.vue'

export default {
	components: {
		AppHeader,
		AppComingSoon,
		AppProdotti,
		AppFooter,
	}
}
</script>
<template>
	<!-- logo e v-for link -->

	<AppHeader />

	<main>

		<AppComingSoon />

		<!-- sezione (v-for ) con tipologie prodotti e icone -->
		<AppProdotti />

	</main>
	<!-- due fasce di cui una con background image -->
	<AppFooter />
</template>

<style scoped></style>
