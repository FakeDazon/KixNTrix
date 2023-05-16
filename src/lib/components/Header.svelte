<script>
    import Cart from "./Cart.svelte";
import Logo from "./Logo.svelte";
</script>

<header>
  <div class="header-inner">
    <div class="left">
      <Logo size={70}/>
    </div>
    <div class="center">
      <a href="../shop/kix">KIX</a>
      <a href="../shop/clothes">CLOTHES</a>
    </div>
    <div class="right">
      <a href="" class="button">
          <Cart size={35}></Cart>
      </a>
    </div></div>
</header>

<style>
  header {
    background: var(--purp);
    width: 100%;
    height: 100px;
    clip-path: polygon(
      0 100%,
      calc(0% + 450px) calc(100% - 15px),
      calc(0% + 445px) calc(100% - 0px),
      max(100%, 842px) calc(100% - 15px),
      100% 0,
      0 0
    );
    display: flex;
    justify-content: space-between;
    padding-bottom: 10px;
    box-sizing: border-box;
    position: fixed;
    top:0;
    z-index: 100;
  }
.header-inner {
    margin: auto;
    width: min(1200px, 90vw);
    height: 100%;
    display: flex;
    justify-content: space-between;
}
  .left,
  .right {
    width: 30%;
    height: 100%;
  }
  .center {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 50px;
  }
  .left {
    display: flex;
    padding-left: 15px;
    box-sizing: border-box;
    align-items: center;
  }
  .right {
    display: flex;
    padding-right: 25px;
    justify-content: flex-end;
    box-sizing: border-box;
    align-items: center;
  }
  a.button {
    display: flex;
    width: 30px;
    height: 30px;
    justify-content: center;
    align-items: center;
    
    padding: 15px 10px
  }
</style>
