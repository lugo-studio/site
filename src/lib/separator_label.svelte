<script lang="ts">
  let { label, width } = $props();
</script>

<div>
  <hr
    class="h-px border-t-0 bg-transparent bg-gradient-to-r from-transparent via-ctp-text to-transparent"
  />
  <div
    class="-my-3 h-fit {width} text-center justify-self-center-safe bg-ctp-mantle"
  >
    {label}
  </div>
</div>
