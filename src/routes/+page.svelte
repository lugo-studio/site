<script lang="ts">
  import Page from "$lib/page.svelte";
</script>

<Page delimiter="" subtitle="" {header} {content} />

{#snippet header()}
  <div class="text-5xl text-center text-ctp-subtext0">Hello hello, friends.</div>
{/snippet}

{#snippet content()}
  <div class="columns-auto gap-10 text-center">
    <a
      href="https://github.com/Lugo-Studio"
      aria-label="GitHub"
      class="text-ctp-text"
    >
      <span class="text-8xl icon-[line-md--github]"></span>
    </a>
    <a
      href="https://x.com/GTLugo"
      aria-label="Twitter (X)"
      class="text-ctp-text"
    >
      <span class="text-8xl icon-[line-md--twitter-x]"></span>
    </a>
    <a
      href="https://www.linkedin.com/in/gabriel-a-lugo/"
      aria-label="LinkedIn"
      class="text-ctp-text"
    >
      <span class="text-8xl icon-[line-md--linkedin]"></span>
    </a>
  </div>
  <div class="px-8"></div>
{/snippet}
