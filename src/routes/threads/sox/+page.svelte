<script>
    import ClassicMain from "$lib/assets/clothing/FINELINESOX.png"
</script>
<div class="main">
    <div class="column">
        <div class="card-image">
            <img src={ClassicMain} alt="">
        </div>
    </div>
    <div class="column">
        <h1>FINELINE SOX</h1>
        <h3>$15.00</h3>
        <p>keep your feet grounded in our classic fineline sox. </p>
        <a class="button button-cyan">ADD TO CART</a>
    </div>
</div>

<svelte:head>
	<title>FINELINE SOX</title>
</svelte:head>

<style>
	.card-image {
		width: 100%;
		height: 400px;
		position: relative;
	}
	.card-image img {
    position: absolute;
		width: 100%;
		height: 100%;
		object-fit: contain;
		transition: all .2s var(--snap-easing);
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
    .main {
        display: flex;
        justify-content: center;
    width: min(1200px, 90vw);
    margin: auto;
    padding-top: 100px;
    gap: 50px;
    padding-bottom: 250px;
    }
    .column {
        width: 100%;
    }
    h3{
        font-family: "Sligoil";
        font-size: 30px;
    }
</style>