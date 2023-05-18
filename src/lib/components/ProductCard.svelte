<script>
	export let img;
  export let secondImg = img;
	export let title = "Placeholder";
	export let price = "$0.00";
	export let href = "";
</script>

<a {href} class="card-main">
	<div class="card-image">
		<img class="img-1" src={img} alt="" />
		<img class="img-2" src={secondImg} alt="" />
	</div>
	<div class="card-details">
		<h3>{title}</h3>
		<h4>{price}</h4>
	</div>
</a>

<style>
	.card-image {
		width: 100%;
		height: 400px;
		position: relative;
	}
	@media (max-width: 1000px) {
	.card-image {
		height: 40vw;
	}

	}
	@media (max-width: 600px) {
	.card-image {
		height: 80vw;
	}

	}
	.card-image img {
    position: absolute;
		width: 100%;
		height: 100%;
		object-fit: contain;
		transition: all .2s var(--snap-easing);
	}
	a {
		all: initial;
		cursor: pointer;
	}
	a:before {
		all: initial;
	}
	h3 {
		text-align: center;
		margin-bottom: 0;
		text-transform: uppercase;
	}
	h4 {
		text-align: center;
		margin-top: 5px;
    color: var(--purp)
	}
	.card-image::before {
		content: "";
		background: rgb(209, 206, 212);
		position: absolute;
		left: 10px;
		top: 10px;
		right: 10px;
		bottom: 10px;
		z-index: -10;
		clip-path: polygon(
			45px 75px,
			25px calc(100% - 35px),
			calc(100% - 35px) calc(100% - 20px),
			calc(100% - 50px) 45px
		);
		transition: all 0.3s var(--snap-easing);
	}
	.card-main:hover .card-image::before,
	.card-main:focus .card-image::before {
		background: rgb(184, 182, 189);
		clip-path: polygon(
			25px 55px,
			55px calc(100% - 25px),
			calc(100% - 45px) calc(100% - 50px),
			calc(100% - 25px) 75px
		);
	}
	.card-main:focus .card-image img, .card-main:hover .card-image img {
		transform: scale(105%) translateY(-10px);
	}
  .img-2 {
    opacity: 0;
  }
  .card-main:focus .img-1, .card-main:hover .img-1 {
    opacity: 0;
  }
  .card-main:focus .img-2, .card-main:hover .img-2 {
    opacity: 1;
  }
</style>
