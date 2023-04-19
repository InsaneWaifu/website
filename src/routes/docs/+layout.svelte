<script>
    import { AppShell } from "@skeletonlabs/skeleton";
    import DocsPageLink from "./DocsPageLink.svelte";

</script>
<AppShell>
	<svelte:fragment slot="sidebarLeft">
        <div class="variant-ghost-surface sidebar flex items-center flex-col">
            <h3 class="underline mb-4">Docs</h3>
            <DocsPageLink link="/docs/usage" text="Basic usage"/>
            <DocsPageLink link="/docs/ratings" text="Ratings"/>
        </div>
    </svelte:fragment>
    <slot></slot>
</AppShell>
<style lang="postcss">
    .sidebar {
        height: 100%;
        width: 10vw;
        border: none !important;
        box-shadow: none !important;
    }
</style>