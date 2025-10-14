<script lang="ts">
  import {
    Navbar,
    NavBrand,
    NavHamburger,
    NavLi,
    NavUl,
  } from "flowbite-svelte";
</script>

<header class="md:pt-4 md:px-4">
  <Navbar class="rounded-lg">
    <NavBrand href="/">
      <img
        src="/assets/favicon.png"
        class="me-3 h-6 sm:h-9"
        alt="Flowbite Logo"
      />
    </NavBrand>
    <NavHamburger />
    <NavUl classes={{ ul: "rounded-lg bg-ctp-crust! md:bg-transparent!" }}>
      <!-- <NavLi href="/">
        <span class="md:text-2xl font-[Oxanium] font-bold">Home</span>
      </NavLi>
      <NavLi href="/">
        <span class="md:text-2xl font-[Oxanium] font-bold">About</span>
      </NavLi> -->
      <NavLi href="https://gtlugo.com">
        <span class="md:text-2xl font-[Oxanium] font-bold">Blog</span>
      </NavLi>
    </NavUl>
  </Navbar>
</header>
