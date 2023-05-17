<script>
    import HeroImage from "$lib/assets/herohome.png";
    import ProductCard from "$lib/components/ProductCard.svelte";
  import SoxMain from "$lib/assets/clothing/FINELINESOX.png"
  import SoxSecond from "$lib/assets/clothing/FINELINESOX2.png"
  import GalaxyMain from "$lib/assets/clothing/Galaxy_Shirt/main.png"
  import GalaxySecond from "$lib/assets/clothing/Galaxy_Shirt/second.png"
  import BeanieMain from "$lib/assets/clothing/Tie_Die_Beanie/main.png"
  import BeanieSecond from "$lib/assets/clothing/Tie_Die_Beanie/second.png"
  import CorduroyMain from "$lib/assets/clothing/Corduroy_Cap/main.png"
  import CorduroySec from "$lib/assets/clothing/Corduroy_Cap/second.png"
  import HoodieMain from "$lib/assets/clothing/Tie_Die_Hoodie/main.png"
  import HoodieSec from "$lib/assets/clothing/Tie_Die_Hoodie/second.png"
  import BomberMain from "$lib/assets/clothing/Bomber/main.png"
  import BomberSec from "$lib/assets/clothing/Bomber/second.png"
  import TrunxMain from "$lib/assets/clothing/trunx/main.png"
  import TrunxSec from "$lib/assets/clothing/trunx/second.png"
  </script>
  
  <div style="height:100px"></div>
  <h2>ALL THREADS</h2>
  
  <div class="product-grid">
    <ProductCard href={"../threads/galaxyshirt"} img={GalaxyMain} secondImg={GalaxySecond} title={"GALAXY SHIRT"} price={"$50.00"}></ProductCard>
    <ProductCard href={"../threads/beanie"} img={BeanieMain} secondImg={BeanieSecond} title={"TIE DYE BEANIE"} price={"$20.00"}></ProductCard>
    <ProductCard href={"../threads/sox"} img={SoxMain} secondImg={SoxSecond} title={"FINE LINE SOX"} price={"$15.00"}></ProductCard>
    <ProductCard href={"../threads/corduroycap"} img={CorduroyMain} secondImg={CorduroySec}  title={"CORDUROY CAP"} price={"$20.00"}></ProductCard>
    <ProductCard href={"../threads/hoodie"} img={HoodieMain} secondImg={HoodieSec} title={"TIE DYE HOODIE"} price={"$80.00"}></ProductCard>
    <ProductCard href={"../threads/bomber"} img={BomberMain} secondImg={BomberSec} title={"CLASSIC BOMBER"} price={"$90.00"}></ProductCard>
    <ProductCard href={"../threads/sweettrunx"} img={TrunxMain} secondImg={TrunxSec} title={"SWEET BREEZE TRUNX"} price={"$20.00"}></ProductCard>
  </div>
  