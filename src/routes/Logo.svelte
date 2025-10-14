<script lang="ts">
  import Signature from "./Signature.svelte";

  const name = ["LUGO", "STUDIO"];
</script>

<!-- https://stackoverflow.com/questions/43496495/text-shadow-in-safari-getting-cut-off-not-rendering-beyond-element-border -->
<div class="mx-auto relative w-fit select-none">
  <div
    class="translate-z-0 absolute right-3 w-22 md:right-8 md:w-40 aspect-square drop-shadow-[0.1rem_0.1rem_0.05rem_black]"
  >
    <Signature />
  </div>
  <div class="translate-z-0 grid grid-rows-2 gap-2">
    {#each name as sub, _}
      <h1
        class="translate-z-0 mx-auto font-[Lugo] text-8xl md:text-[11rem] leading-[0.6] drop-shadow-[0.2rem_0.3rem_0.1rem_rgba(1,1,1,1)] md:drop-shadow-[0.2rem_0.3rem_0.15rem_rgba(1,1,1,1)]"
      >
        <div
          class="translate-z-0 grid grid-cols-6 gap-0 drop-shadow-[0.2rem_0.3rem_0.1rem_rgba(1,1,1,1)]"
        >
          {#each sub as char, _}
            <span class="logo-gradient">{char}</span>
          {/each}
        </div>
      </h1>
    {/each}
  </div>
</div>

<style>
  .logo-gradient {
    --color-shine: #e1e5f2;
    --color-shadow: #48557a;

    background-image: linear-gradient(
      135deg,
      var(--color-shine),
      var(--color-shadow)
    );
    background-clip: text;
    color: transparent;
  }
</style>
