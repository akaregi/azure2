<script lang="ts">
  import { fly } from "svelte/transition";
  export let refresh = "";
</script>

{#key refresh}
  <div in:fly={{ x: -10, duration: 250, delay: 250 }} out:fly={{ x: 10, duration: 250 }}>
    <slot />
  </div>
{/key}
