<script lang="ts">
  let { title = "Lugo Studio", delimiter = " | ", subtitle } = $props();
</script>

<svelte:head>
  <title>{title}{delimiter}{subtitle}</title>
</svelte:head>

<img
  src="/lugo_studio_cat_pure_borderless.png"
  alt="Lugo Studio"
  class="drop-shadow-xl/100 justify-self-center-safe"
/>
