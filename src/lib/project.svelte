<script lang="ts">
  import { Link } from 'carbon-components-svelte';
  import { LogoGithub } from 'carbon-icons-svelte';

  export let title: string;
  export let description: string = '';
  export let gitlink: string;
  export let gitname: string;
</script>

<div class="w-full bg-gradient-to-b from-#f2f2f2 to-#f8f8f8  p-10 rounded-3xl grid gap-10">
  <p class="font-semibold text-3xl">{title}</p>

  <p>
    <slot />
    {description}
  </p>

  <div class="flex items-center gap-10px">
    <Link target="_blank" href={gitlink}>
      {gitname}
    </Link>
    <LogoGithub />
  </div>
</div>
