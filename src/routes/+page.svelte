<script>
  import HeroImage from "$lib/assets/herohome.png";
  import ProductCard from "$lib/components/ProductCard.svelte";
  import ClassicMain from "$lib/assets/shoes/Classic_Bolt/main.png"
  import ClassicSec from "$lib/assets/shoes/Classic_Bolt/second.png"
  import BlackMain from "$lib/assets/shoes/Classic_Black/main.png"
  import BlackSecond from "$lib/assets/shoes/Classic_Black/second.png"
  import WhiteMain from "$lib/assets/shoes/Classic_White/main.png"
  import WhiteSecond from "$lib/assets/shoes/Classic_White/second.png"
  import SoxMain from "$lib/assets/clothing/FINELINESOX.png"
  import SoxSecond from "$lib/assets/clothing/FINELINESOX2.png"
  import GalaxyMain from "$lib/assets/clothing/Galaxy_Shirt/main.png"
  import GalaxySecond from "$lib/assets/clothing/Galaxy_Shirt/second.png"
  import BeanieMain from "$lib/assets/clothing/Tie_Die_Beanie/main.png"
  import BeanieSecond from "$lib/assets/clothing/Tie_Die_Beanie/second.png"
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
  <ProductCard href={"../kix/signature"} img={ClassicMain} secondImg={ClassicSec} title={"SIGNATURE BOLT"} price={"$60.00"}></ProductCard>
  <ProductCard href={"../kix/classicblack"} img={BlackMain} secondImg={BlackSecond} title={"CLASSIC BLACK BOLT"} price={"$55.00"}></ProductCard>
  <ProductCard href={"../kix/classicwhite"} img={WhiteMain} secondImg={WhiteSecond} title={"CLASSIC WHITE BOLT"} price={"$55.00"}></ProductCard>
</div>

<a class="button button-cyan centered" href="../kix">SHOP ALL KIX</a>
<div style="height:100px"></div>
<h2>TRENDING THREADS</h2>

<div class="product-grid">
  <ProductCard href={"../threads/galaxyshirt"} img={GalaxyMain} secondImg={GalaxySecond} title={"GALAXY SHIRT"} price={"$50.00"}></ProductCard>
  <ProductCard href={"../threads/beanie"} img={BeanieMain} secondImg={BeanieSecond} title={"TIE DIE BEANIE"} price={"$20.00"}></ProductCard>
  <ProductCard href={"../threads/sox"} img={SoxMain} secondImg={SoxSecond} title={"FINE LINE SOX"} price={"$15.00"}></ProductCard>
</div>

<a class="button button-cyan centered" href="../threads">SHOP ALL THREADS</a>

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
