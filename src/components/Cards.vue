<script>
// JS
export default {
	data() {
		return {
			title: "Header",
			cards: [
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$19.99",
					series: "Action Comics",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$3.99",
					series: "American Vampire 1976",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$16.99",
					series: "Aquaman",
					type: "graphic novel",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$2.99",
					series: "Batgirl",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$3.99",
					series: "Batman",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$2.99",
					series: "Batman Beyond",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$3.99",
					series: "Batman/Superman",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$4.99",
					series: "Batman/Superman Annual",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$5.99",
					series: "Batman: The Joker War Zone",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$6.99",
					series: "Batman: Three Jokers",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$4.99",
					series: "Batman: White Knight Presents: Harley Quinn",
					type: "comic book",
				},
				{
					thumb:
						"https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1rehc005isbn_0_3thlluzys44ope0a.jpg",
					price: "$16.99",
					series: "Catwoman",
					type: "graphic novel",
				},
			],
		};
	},
};
</script>

<template>
	<!-- HTML -->
	<div class="bg">
		<div class="container">
			<div v-for="card in cards" class="card">
				<img :src="card.thumb" alt="" />
				<span>{{ card.series }}</span>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
/* CSS */
@use "../assets/scss/partials/mixins" as *;
.bg {
	background-color: #1c1c1c;
	width: 100%;

	display: flex;
	align-items: center;
	padding: 30px 0;
}
h1 {
	color: white;
}
.container {
	@include flex("horizontal");
	flex-wrap: wrap;
	gap: 30px;
}
.card {
	display: flex;
	flex-direction: column;
	align-items: center;
	width: calc(100% / 6 - 30px);
	img {
		width: 100%;
		height: 170px;
		object-fit: cover;
	}
}
span {
	color: white;
	text-align: center;
}
</style>
