<script lang="ts">
  import { SkeletonText } from 'carbon-components-svelte';

  export let prompt: any;
  export let content: any;
</script>

<div class="flex gap-10px items-end">
  <p>
    {prompt}:
    {#if content}
      {content}
    {/if}
  </p>
  {#if !content}
    <SkeletonText class="w-100px! mb-4px!" />
  {/if}
</div>
