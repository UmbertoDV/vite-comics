<script>
import Header from "./components/Header/Header.vue";
import ContentSection from "./components/Main/ContentSection/ContentSection.vue";

export default {
	components: {
		Header,
		ContentSection,
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
	</main>
</template>

<style lang="scss">
/* CSS */
@use "./assets/scss/global.scss";
</style>
