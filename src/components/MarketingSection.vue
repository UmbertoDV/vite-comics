<script>
// JS
export default {
	data() {
		return {
			marketingObj: {
				digitalComics: {
					text: "DIGITAL COMICS",
					img: "./imgs/buy-comics-digital-comics.png",
				},
				merchandise: {
					text: "DC MERCHANDISE",
					img: "./imgs/buy-comics-merchandise.png",
				},
				sub: {
					text: "SUBSCRIPTION",
					img: "./imgs/buy-comics-shop-locator.png",
				},
				comicShop: {
					text: "COMIC SHOP LOCATION",
					img: "./imgs/buy-comics-subscriptions.png",
				},
				powerVisa: {
					text: "DC POWER VISA",
					img: "./imgs/buy-dc-power-visa.svg",
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

<style scoped>
/* CSS */
.bg {
	background-color: #0282f9;
	padding: 20px;
	width: 100%;

	display: flex;
	align-items: center;
}
.bg img {
	width: 50px;
}
h1 {
	color: white;
}
.card {
	display: flex;
	align-items: center;
	gap: 10px;
	color: white;
}
.container {
	display: flex;
	justify-content: space-evenly;
}
</style>
