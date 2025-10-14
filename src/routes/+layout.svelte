<script lang="ts">
  import { Navbar, NavHamburger, NavLi, NavUl } from "flowbite-svelte";
  import "../app.css";
  import Footer from "./Footer.svelte";
  import Logo from "./Logo.svelte";

  let { children } = $props();
</script>

<div class="mx-auto w-full min-h-screen text-ctp-text bg-ctp-base">
  <div class="mx-auto min-h-screen flex flex-col max-w-screen-xl">
    <div class="grow">
      <header>
        <Navbar class="rounded-lg bg-ctp-crust!">
          <NavHamburger />
          <NavUl class="mx-auto bg-ctp-crust!" ulClass="rounded-lg bg-ctp-mantle!">
            <NavLi href="/">Home</NavLi>
            <NavLi href="/">About</NavLi>
            <NavLi href="https://gtlugo.com">Blog</NavLi>
          </NavUl>
        </Navbar>
        <div class="fadeInUp-animation py-16">
          <Logo />
        </div>
      </header>
      <div class="mx-auto">
        <main class="px-8 py-16">
          {@render children?.()}
        </main>
      </div>
    </div>
    <div class="flex-none">
      <Footer />
    </div>
  </div>
</div>

<style>
  /* https://dev.to/tiaeastwood/super-simple-css-animation-for-fade-in-on-page-load-2p8m */

  @keyframes fadeInUp {
    /* start animation, but leave invisible for a bit for it to load */
    0% {
      transform: translateY(25%);
      opacity: 0;
    }

    20% {
      transform: translateY(25%);
      opacity: 0;
    }

    100% {
      transform: translateY(0%);
      opacity: 1;
    }
  }

  .fadeInUp-animation {
    animation: 1s fadeInUp;
  }
</style>
