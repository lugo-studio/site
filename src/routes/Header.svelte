<script lang="ts">
  import { Navbar, NavHamburger, NavLi, NavUl } from "flowbite-svelte";
</script>

<header class="md:pt-4 md:px-4">
  <Navbar class="rounded-lg bg-ctp-crust!">
    <NavHamburger />
    <NavUl
      class="mx-auto bg-ctp-crust!"
      classes={{ ul: "rounded-lg bg-ctp-crust!" }}
    >
      <NavLi href="/">Home</NavLi>
      <NavLi href="/">About</NavLi>
      <NavLi href="https://gtlugo.com">Blog</NavLi>
    </NavUl>
  </Navbar>
</header>
