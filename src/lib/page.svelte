<script lang="ts">
  import Logo from "$lib/logo.svelte";
  import Sep from "$lib/separator.svelte";
  let { title = "Lugo Studio", delimiter = " | ", subtitle, header, content } = $props(); 
</script>

<div
  class="mx-auto absolute top-0 lg:inset-x-50 w-full lg:w-1/2 h-dvh text-ctp-text"
>
  <div class="grid grid-cols-1 gap-10">
    <Logo title={title} delimiter={delimiter} subtitle={subtitle} />
    <Sep />
    <div class="grid grid-cols-1 gap-10">
      {@render header()}
      <Sep />
      {@render content()}
    </div>
  </div>
</div>
<div
  class="-z-1 relative fixed top-0 bg-ctp-mantle mx-auto max-w-full lg:max-w-1/2 h-screen blur-sm"
></div>