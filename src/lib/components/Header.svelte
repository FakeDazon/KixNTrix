<script>
  import Cart from "./Cart.svelte";
  import Logo from "./Logo.svelte";
  import Menu from "./Menu.svelte";
  let visible = false;
</script>

<header>
  <div class="header-inner">
    <div class="left">
      <a class="none" href="../">
        <Logo size={70} />
      </a>
    </div>
    <div class="center">
      <a href="../kix">KIX</a>
      <a href="../threads">THREADS</a>
    </div>
    <div class="right">
      <a href="" class="button">
        <Cart size={35} />
      </a>
    </div>
    <div class="right2">
      <a on:click={()=>{visible = !visible}} on:keypress={()=>{visible = !visible}}  class="button">
        <Menu size={35} />
      </a>
    </div>
  </div>
</header>
<div id="dropdown" class={visible ? "visible" : ""}>
  
  <a href="../kix">KIX</a>
  <a href="../threads">THREADS</a>
  <a href="" class="button button-cyan buttona">
    <Cart size={35} color="black" />
    CART
  </a>
</div>

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
    top: 0;
    z-index: 100;
  }
  #dropdown {
    padding-top: 130px;
    position: fixed;
    width: 100%;
    height: fit-content;
    display: flex;
    justify-content: space-between;
    padding-bottom: 80px;
    z-index: 99;
    gap: 30px;
    align-items: center;
    flex-direction: column;
    background: var(--navy);
    clip-path: polygon(
      0 0,
      calc(0% + 450px) 0,
      calc(0% + 445px) 0,
      max(100%, 842px) 0,
      100% 0,
      0 0
    );
    transition: clip-path 0.4s ease-in-out;
  }
  #dropdown * {
    opacity: 0;
    transition: all 0.3s
  }
  .visible {
    clip-path: polygon(
      0 calc(100% - 30px),
      calc(0% + 450px) calc(100% - 45px),
      calc(0% + 445px) calc(100% - 30px),
      max(100%, 842px) calc(100% - 45px),
      100% 0,
      0 0
    ) !important;

  }
  #dropdown.visible * {
    opacity: 1;
  }
  
  #dropdown.visible *:nth-child(1) {
    transition-delay: 0.2s;
  }
  #dropdown.visible *:nth-child(2) {
    transition-delay: 0.3s;
  }
  #dropdown.visible *:nth-child(3) {
    transition-delay: 0.35s;
  }
  #dropdown a:not(.button-cyan):before {
    background: var(--purp)
  }
  .buttona {
    width: fit-content !important;
    gap: 20px;
    padding: 15px 15px !important;
  }
  @media (min-width: 600px) {
    #dropdown {
      visibility: hidden;
      display: none;
      pointer-events: none;
    }
  }
  .header-inner {
    margin: auto;
    width: min(1200px, 90vw);
    height: 100%;
    display: flex;
    justify-content: space-between;
  }
  .left,
  .right,
  .right2 {
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
  .right,
  .right2 {
    display: flex;
    padding-right: 25px;
    justify-content: flex-end;
    box-sizing: border-box;
    align-items: center;
  }
  .right2 {
    display: none;
  }
  a.button {
    display: flex;
    width: 30px;
    height: 30px;
    justify-content: center;
    align-items: center;

    padding: 15px 10px;
  }

  .none {
    all: initial;
    cursor: pointer;
  }
  .none:before {
    all: initial;
  }

  @media (max-width: 600px) {
    .center {
      display: none;
    }
    .right {
      display: none;
    }
    .right2 {
      display: flex;
    }
  }
</style>
