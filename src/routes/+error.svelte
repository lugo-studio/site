<script lang="ts">
  import Logo from "$lib/logo.svelte";
  import Sep from "$lib/separator.svelte";
  import SepLabel from "$lib/separator_label.svelte";
  import { page } from "$app/state";
</script>

<div
  class="mx-auto absolute top-0 lg:inset-x-50 w-full lg:w-1/2 h-dvh text-ctp-text"
>
  <div class="grid grid-cols-1 gap-10">
    <Logo subtitle={page.error?.message} />
    <Sep />
    <div class="grid grid-cols-1 gap-10">
      <div class="text-5xl text-center">Oh nyo~!</div>
      <SepLabel label={page.error?.message} width={"w-1/4"} />
    </div>
  </div>
</div>
<div
  class="-z-1 relative fixed top-0 bg-ctp-mantle mx-auto max-w-full lg:max-w-1/2 h-screen blur-sm"
></div>
