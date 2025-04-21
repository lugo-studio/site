<script lang="ts">
  import Page from "$lib/page.svelte";
</script>

<Page delimiter="" subtitle="" {header} {content} />

{#snippet header()}
  <div class="text-5xl text-center">Hello hello, friends.</div>
{/snippet}

{#snippet content()}
  <div class="px-8"></div>
{/snippet}
