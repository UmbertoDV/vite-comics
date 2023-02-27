<script>
import Header from "./components/Header/Header.vue";
import ContentSection from "./components/Main/ContentSection/ContentSection.vue";
import MarketingSection from "./components/Main/MarketingSection/MarketingSection.vue";
import Footer from "./components/Footer/Footer.vue";

export default {
	components: {
		Header,
		ContentSection,
		MarketingSection,
		Footer,
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
		<ContentSection></ContentSection>
		<MarketingSection></MarketingSection>
	</main>
	<footer>
		<Footer></Footer>
	</footer>
</template>

<style lang="scss">
/* CSS */
@use "./assets/scss/global.scss";
</style>
