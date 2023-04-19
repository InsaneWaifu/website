<script lang="ts">
  // The ordering of these imports is critical to your app working properly
  import "@skeletonlabs/skeleton/themes/theme-gold-nouveau.css";
  // If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
  import "@skeletonlabs/skeleton/styles/all.css";
  // Most of your app wide CSS should be put in this file
  import "../app.postcss";
  import { AppShell, AppBar } from "@skeletonlabs/skeleton";
</script>

<!-- App Shell -->
<AppShell>
  <svelte:fragment slot="header">
    <!-- App Bar -->	
    <AppBar>
      <svelte:fragment slot="lead">
        <a href="/" rel="noreferrer">
          <strong class="text-xl uppercase">Chesscord</strong>
        </a>
      </svelte:fragment>
      <svelte:fragment slot="trail">
        <a
          class="btn btn-sm variant-ghost-surface"
          href="https://discord.com/api/oauth2/authorize?client_id=1097269752696672256&permissions=280576&scope=bot%20applications.commands"
          target="_blank"
          rel="noreferrer"
        >
          Add to server
        </a>
      </svelte:fragment>
    </AppBar>
  </svelte:fragment>
  <!-- Page Route Content -->
  <slot />
</AppShell>
