<script lang="ts">
  let { title = "Lugo Studio", delimiter = " | ", subtitle } = $props();
</script>

<svelte:head>
  <title>{title}{delimiter}{subtitle}</title>
</svelte:head>

<img
  src="/assets/images/branding/cat_pure_borderless_sha2.png"
  alt="Lugo Studio"
  class="justify-self-center-safe"
/>
