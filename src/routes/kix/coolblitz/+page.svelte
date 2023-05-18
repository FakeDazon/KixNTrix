<script>
    import ClassicMain from "$lib/assets/shoes/Cool_Blitz/main.png"
</script>
<div class="main">
    <div class="column">
        <div class="card-image">
            <img src={ClassicMain} alt="">
        </div>
    </div>
    <div class="column">
        <h1>COOL BLITZ BOLT</h1>
        <h3>$60.00</h3>
        <p>dive right into the summer fun with a limited edition pair of kix. sport the signature kix n trix design with an all new ocean colorway.</p>
        <a class="button button-cyan">ADD TO CART</a>
    </div>
</div>

<svelte:head>
	<title>COOL BLITZ BOLT KIX</title>
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
    width: min(1200px, calc(90vw - 50px));
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
    @media (max-width: 1000px) {

        .main {
        display: flex;
        justify-content: center;
        flex-direction: column;
    }
    }
</style>