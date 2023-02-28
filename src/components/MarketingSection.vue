<script>
// JS
export default {
	data() {
		return {
			marketingObj: {
				digitalComics: {
					text: "DIGITAL COMICS",
					img: "/buy-comics-digital-comics.png",
				},
				merchandise: {
					text: "DC MERCHANDISE",
					img: "/buy-comics-merchandise.png",
				},
				sub: {
					text: "SUBSCRIPTION",
					img: "/buy-comics-shop-locator.png",
				},
				comicShop: {
					text: "COMIC SHOP LOCATION",
					img: "/buy-comics-subscriptions.png",
				},
				powerVisa: {
					text: "DC POWER VISA",
					img: "/buy-dc-power-visa.svg",
				},
			},
		};
	},
};
</script>

<template>
	<!-- HTML -->
	<div class="bg">
		<div class="container">
			<div v-for="card in marketingObj" class="card">
				<img :src="card.img" alt="" />
				<span>{{ card.text }}</span>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/mixins" as *;
.bg {
	background-color: #0282f9;
	padding: 20px;
	width: 100%;

	@include flex("vertical");
}
.bg img {
	width: 50px;
}
h1 {
	color: white;
}
.card {
	@include flex("vertical");
	gap: 10px;
	color: white;
}
.container {
	display: flex;
	justify-content: space-evenly;
}
</style>
