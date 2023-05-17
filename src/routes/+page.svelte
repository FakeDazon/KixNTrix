<script>
  import HeroImage from "$lib/assets/herohome.png";
  import ProductCard from "$lib/components/ProductCard.svelte";
</script>

<section class="hero">
  <div class="hero-inner">
    <div class="hero-section">
      <h1><span class="sunsetGradient">FRESH</span> SUMMER KIX</h1>
      <p>
        chill out in the heat with the freshest kix around. check out the latest
        drops from our 2023 summer collection.
      </p>
      <a class="button button-cyan" href="../collections/summer2023">SHOP THE COLLECTION</a>
    </div>
    <div class="hero-image"><img src={HeroImage} alt="" /></div>
  </div>
</section>

<h2>CLASSIC KIX</h2>

<div class="product-grid">
  <ProductCard title={"CLASSIC BOLT"} price={"$59.99"}></ProductCard>
  <ProductCard title={"CLASSIC BLACK BOLT"} price={"$54.99"}></ProductCard>
  <ProductCard title={"CLASSIC WHITE BOLT"} price={"$54.99"}></ProductCard>
</div>

<style>
  .sunsetGradient {
    background-image: radial-gradient(
        200% 100% at bottom,
        white 5%,
        rgb(255, 133, 133) 15%,
        transparent 100%
      ),
      linear-gradient(to right, #8400ff 0%, #ff23b6 50%, #ff9735 80%);

    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    padding-right: 20px;
    margin-right: -20px;
  }
  a {
    margin-top: 20px;
  }
</style>
