<script>
import Header from "./components/Header.vue";
import ContentSection from "./components/ContentSection.vue";
import MarketingSection from "./components/MarketingSection.vue";
import Footer from "./components/Footer.vue";
import Cards from "./components/Cards.vue";

export default {
	components: {
		Header,
		ContentSection,
		MarketingSection,
		Footer,
		Cards,
	},
};
</script>

<template>
	<!-- HTML -->
	<header>
		<div class="container">
			<Header></Header>
		</div>
	</header>
	<main>
		<Cards></Cards>
		<ContentSection></ContentSection>
		<MarketingSection></MarketingSection>
	</main>
	<footer>
		<Footer></Footer>
	</footer>
</template>

<style lang="scss">
/* CSS */
@use "./assets/scss/global.scss" as *;
</style>
