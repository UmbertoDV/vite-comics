<script>
// JS

export default {
	data() {
		return {
			title: "Header",
			headerObj: {
				characters: {
					text: "characters",
					url: "#",
				},
				comics: {
					text: "comics",
					url: "#",
				},
				movies: {
					text: "movies",
					url: "#",
				},
				tv: {
					text: "tv",
					url: "#",
				},
				games: {
					text: "games",
					url: "#",
				},
				collectibles: {
					text: "collectibles",
					url: "#",
				},
				video: {
					text: "video",
					url: "#",
				},
				fans: {
					text: "fans",
					url: "#",
				},
				news: {
					text: "news",
					url: "#",
				},
				shop: {
					text: "shop",
					url: "#",
				},
			},
		};
	},
};
</script>

<template>
	<!-- HTML -->
	<div class="header">
		<div class="logo">
			<img src="./imgs/dc-logo.png" alt="" />
		</div>
		<nav>
			<ul>
				<li v-for="headerText in headerObj">
					<a :href="headerText.url">{{ headerText.text.toUpperCase() }}</a>
				</li>
			</ul>
		</nav>
	</div>
</template>

<style lang="scss" scoped>
/* CSS */
@use "../../assets/scss/mixins";
.header {
	padding: 15px 0;
	@include flex;
}
</style>
