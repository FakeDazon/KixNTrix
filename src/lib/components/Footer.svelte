<script>
  import Ig from "./IG.svelte";
import LogoWhite from "./Logo-White.svelte";
</script>

<footer>
  <div class="footer-inner">
    <div class="footer-section footer-logo">
      <LogoWhite size={70} />
      <a class="button button-white"  href="ig"><Ig color={"#004"} size={25}></Ig></a>
    </div>
    <div class="footer-section">
      <h3>SHOP</h3>
      <a href="../">HOME</a>
      <a href="../shop/kix">KIX</a>
      <a href="../shop/clothes">CLOTHES</a>
    </div>
    <div class="footer-section">
      <h3>COLLECTIONS</h3>
      <a href="../collections/summer2023">SUMMER 2023</a>
    </div>
    <div class="footer-section">
      <h3>COMPANY</h3>
      <a href="../about">ABOUT</a>
    </div>
</footer>

<style>
  footer {
    background: var(--navy);
    width: 100%;
    clip-path: polygon(
      min(calc(100% - 840px), 0%) 0,
      calc(100% - 445px) 30px,
      calc(100% - 450px) 15px,
      100% 50px,
      100% 100%,
      0 100%
    );
    display: flex;
    justify-content: space-between;
    padding: 50px;
    padding-top: 100px;
    box-sizing: border-box;
    margin-top: 50px;
  }
.footer-inner {
    margin: auto;
    width: min(1200px, 90vw);
    height: 100%;
    display: flex;
    justify-content: space-between;
}
.footer-section {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: start;
  gap: 10px;
}
.footer-logo{
  align-items: center;
  gap: 20px;
}
h3{
  color: var(--whit);
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
  a:not(.button){
    all: initial;
    font-family: 'Sligoil';
    cursor: pointer;
    color: white;
  }
  a:not(.button):hover,a:not(.button):focus {
    color: var(--cyan);
  }
  a.button {
    padding: 0;
    width: 30px; height: 35px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>
