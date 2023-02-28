<script>
// JS
</script>

<template>
	<!-- HTML -->
	<div class="bg">
		<div class="container">
			<div class="left-footer">
				<div class="first-col">
					<h2>DC COMICS</h2>
					<ul>
						<li><a href="#">Characters</a></li>
						<li><a href="#">Comics</a></li>
						<li><a href="#">Movies</a></li>
						<li><a href="#">TV</a></li>
						<li><a href="#">Games</a></li>
						<li><a href="#">Videos</a></li>
						<li><a href="#">News</a></li>
					</ul>
					<h2>SHOP</h2>
					<ul>
						<li><a href="#">Characters</a></li>
						<li><a href="#">Comics</a></li>
					</ul>
				</div>
				<div class="sec-col">
					<h2>DC COMICS</h2>
					<ul>
						<li><a href="#">Characters</a></li>
						<li><a href="#">Comics</a></li>
						<li><a href="#">Movies</a></li>
						<li><a href="#">TV</a></li>
						<li><a href="#">Games</a></li>
						<li><a href="#">Videos</a></li>
						<li><a href="#">News</a></li>
					</ul>
				</div>
				<div class="third-col">
					<h2>DC COMICS</h2>
					<ul>
						<li><a href="#">Characters</a></li>
						<li><a href="#">Comics</a></li>
						<li><a href="#">Movies</a></li>
						<li><a href="#">TV</a></li>
						<li><a href="#">Games</a></li>
						<li><a href="#">Videos</a></li>
						<li><a href="#">News</a></li>
					</ul>
				</div>
			</div>
			<div class="right-footer">
				<div class="img-bg">
					<img src="../assets/imgs/dc-logo-bg.png" alt="" />
				</div>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/mixins" as *;
.bg {
	background-image: url("../assets/imgs/footer-bg.jpg");
	background-size: cover;
	width: 100%;

	@include flex("vertical");
}
h1 {
	color: white;
}
.container {
	display: flex;
	justify-content: space-between;
	gap: 20px;
	.left-footer {
		display: flex;
	}
}
</style>
