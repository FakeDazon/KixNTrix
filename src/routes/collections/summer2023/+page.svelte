<script>
    import HeroImage from "$lib/assets/herohome.png";
    import ProductCard from "$lib/components/ProductCard.svelte";
    import ClassicMain from "$lib/assets/shoes/Classic_Bolt/main.png"
    import ClassicSec from "$lib/assets/shoes/Classic_Bolt/second.png"
    import BlackMain from "$lib/assets/shoes/Classic_Black/main.png"
    import BlackSecond from "$lib/assets/shoes/Classic_Black/second.png"
    import WhiteMain from "$lib/assets/shoes/Classic_White/main.png"
    import WhiteSecond from "$lib/assets/shoes/Classic_White/second.png"
    import SweetMain from "$lib/assets/shoes/Sweet_Breeze/main.png"
    import SweetSec from "$lib/assets/shoes/Sweet_Breeze/second.png"
    import CoolMain from "$lib/assets/shoes/Cool_Blitz/main.png"
    import CoolSec from "$lib/assets/shoes/Cool_Blitz/second.png"
    import CampMain from "$lib/assets/shoes/Campsite/main.png"
    import CampSec from "$lib/assets/shoes/Campsite/second.png"
  import TrunxMain from "$lib/assets/clothing/trunx/main.png"
  import TrunxSec from "$lib/assets/clothing/trunx/second.png"
  </script>
  
  <div style="height:100px"></div>
  <h2>SUMMER 2023 COLLECTION</h2>
  
  <div class="product-grid">
    <ProductCard href={"../kix/campsite"} img={CampMain} secondImg={CampSec} title={"CAMPSITE BOLT"} price={"$60.00"}></ProductCard>
    <ProductCard href={"../kix/coolblitz"} img={CoolMain} secondImg={CoolSec} title={"COOL BLITZ BOLT"} price={"$60.00"}></ProductCard>
    <ProductCard href={"../kix/sweetbreeze"} img={SweetMain} secondImg={SweetSec} title={"SWEET BREEZE BOLT"} price={"$60.00"}></ProductCard>
    <ProductCard href={"../threads/sweettrunx"} img={TrunxMain} secondImg={TrunxSec} title={"SWEET BREEZE TRUNX"} price={"$20.00"}></ProductCard>
  </div>
  