<script lang="ts">
  import Page from "$lib/page.svelte";
</script>

<Page delimiter="" subtitle="" {header} {content} />

{#snippet header()}
  <div class="text-5xl text-center">Hello hello, friends.</div>
{/snippet}

{#snippet content()}
  <div class="columns-auto gap-10 text-center">
    <a href="https://github.com/Lugo-Studio" aria-label="GitHub">
      <span class="text-8xl icon-[octicon--mark-github-24]"></span>
    </a>
    <a href="https://x.com/GTLugo" aria-label="Twitter (X)">
      <span class="text-8xl icon-[line-md--twitter-x]"></span>
    </a>
  </div>
  <div class="px-8"></div>
{/snippet}
