<script>
  import {
    Header,
    SideNav,
    SideNavItems,
    SideNavMenu,
    SideNavMenuItem,
    SideNavLink,
    SideNavDivider,
    SkipToContent,
    Content,
    Grid,
    Row,
    Column,
    HeaderUtilities,
    HeaderGlobalAction,
    HeaderAction,
    HeaderPanelLinks,
    HeaderPanelLink,
    HeaderPanelDivider
  } from 'carbon-components-svelte';
  import Logout from 'carbon-icons-svelte/lib/Logout.svelte';
  import { SkeletonText } from 'carbon-components-svelte';
  import { goto } from '$app/navigation';

  import 'carbon-components-svelte/css/white.css';
  import './styles.css';
  import 'virtual:uno.css';
  import UserAvatarFilledAlt from 'carbon-icons-svelte/lib/UserAvatarFilledAlt.svelte';
  import { browser } from '$app/environment';

  let isSideNavOpen = false;
  let isOpen1 = false;
</script>

<main class="mx-10">
  <slot />
</main>
